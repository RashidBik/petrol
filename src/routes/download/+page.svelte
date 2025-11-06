<script>
  let downloadInfo = {
    version: "1.3.0",
    size: "110 مگابایت",
    releaseDate: "1402/10/15",
    requirements: [
      "سیستم عامل: WINDOWS 10، 11 ",
      "پردازنده: Intel Core i5 یا معادل آن",
      "حافظه رم: حداقل 4 گیگابایت",
      "فضای ذخیره‌سازی: 256 مگابایت فضای آزاد"
    ]
  };

  let downloadSteps = [
    {
      step: 1,
      title: "دانلود فایل نصب",
      description: "فایل نصب را از لینک زیر دانلود کنید"
    },
    {
      step: 2,
      title: "اجرای فایل نصب",
      description: "فایل اجرایی را باز کرده و مراحل نصب را طی کنید"
    },
    {
      step: 3,
      title: "فعال‌سازی نرم‌افزار",
      description: "نرم‌افزار را اجرا کرده و با اطلاعات خود وارد شوید"
    }
  ];
</script>

<svelte:head>
  <title>دانلود نرم‌افزار ثبت و آنالیز داده‌های تانک تیل</title>
</svelte:head>

<div class="download-page">
  <div class="container">
    <header class="page-header">
      <h1>دانلود نرم‌افزار</h1>
      <p>نسخه کامل نرم‌افزار ثبت و آنالیز داده‌های تانک تیل</p>
    </header>

    <div class="download-content">
      <div class="download-card">
        <div class="download-info">
          <h2>نرم‌افزار ثبت و آنالیز داده‌های تانک تیل</h2>
          <div class="version-info">
            <div class="info-item">
              <span class="label">نسخه:</span>
              <span class="value">{downloadInfo.version}</span>
            </div>
            <div class="info-item">
              <span class="label">حجم:</span>
              <span class="value">{downloadInfo.size}</span>
            </div>
            <div class="info-item">
              <span class="label">تاریخ انتشار:</span>
              <span class="value">{downloadInfo.releaseDate}</span>
            </div>
          </div>

          <div class="download-button-container">
            <a href="/downloads/tank-teel-analyzer-v1.0.0.exe" class="btn btn-download" download>
              <span class="download-icon">⬇️</span>
              دانلود نرم‌افزار
            </a>
          </div>

          <div class="system-requirements">
            <h3>سیستم مورد نیاز</h3>
            <ul>
              {#each downloadInfo.requirements as requirement}
                <li>{requirement}</li>
              {/each}
            </ul>
          </div>
        </div>
      </div>

      <div class="installation-steps">
        <h2>راهنمای نصب</h2>
        <div class="steps-container">
          {#each downloadSteps as step}
            <div class="step">
              <div class="step-number">{step.step}</div>
              <div class="step-content">
                <h3>{step.title}</h3>
                <p>{step.description}</p>
              </div>
            </div>
          {/each}
        </div>
      </div>

      <div class="support-section">
        <h2>نیاز به کمک دارید؟</h2>
        <p>در صورت بروز هرگونه مشکل در دانلود یا نصب نرم‌افزار، با پشتیبانی فنی تماس بگیرید.</p>
        <div class="support-contacts">
          <a href="mailto:hcrgroup.info@gmail.com" class="support-link">📧 hcrgroup.info@gmail.com</a>
          <a href="tel:+93795552579" class="support-link">📞 +93795552579</a>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .download-page {
    padding: 60px 0;
    background-color: #f8f9fa;
    min-height: 100vh;
  }

  .page-header {
    text-align: center;
    margin-bottom: 50px;
  }

  .page-header h1 {
    font-size: 2.5rem;
    color: #1a365d;
    margin-bottom: 15px;
  }

  .page-header p {
    font-size: 1.2rem;
    color: #4a5568;
  }

  .download-content {
    max-width: 800px;
    margin: 0 auto;
  }

  .download-card {
    background: white;
    border-radius: 12px;
    padding: 40px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    margin-bottom: 40px;
  }

  .download-card h2 {
    color: #1a365d;
    margin-bottom: 25px;
    text-align: center;
    font-size: 1.8rem;
  }

  .version-info {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-bottom: 30px;
  }

  .info-item {
    display: flex;
    justify-content: space-between;
    padding: 15px;
    background: #f7fafc;
    border-radius: 6px;
  }

  .label {
    font-weight: 600;
    color: #4a5568;
  }

  .value {
    color: #1a365d;
    font-weight: 600;
  }

  .download-button-container {
    text-align: center;
    margin: 30px 0;
  }

  .btn-download {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #3182ce;
    color: white;
    padding: 15px 30px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s ease;
  }

  .btn-download:hover {
    background: #2c5aa0;
    transform: translateY(-2px);
  }

  .download-icon {
    font-size: 1.2rem;
  }

  .system-requirements {
    margin-top: 30px;
    padding-top: 20px;
    border-top: 1px solid #e2e8f0;
  }

  .system-requirements h3 {
    color: #1a365d;
    margin-bottom: 15px;
  }

  .system-requirements ul {
    list-style-type: none;
  }

  .system-requirements li {
    padding: 8px 0;
    position: relative;
    padding-right: 20px;
  }

  .system-requirements li::before {
    content: "•";
    color: #3182ce;
    font-weight: bold;
    position: absolute;
    right: 0;
  }

  .installation-steps {
    background: white;
    border-radius: 12px;
    padding: 40px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    margin-bottom: 40px;
  }

  .installation-steps h2 {
    color: #1a365d;
    margin-bottom: 30px;
    text-align: center;
  }

  .steps-container {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }

  .step {
    display: flex;
    gap: 20px;
    align-items: flex-start;
  }

  .step-number {
    background: #3182ce;
    color: white;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    flex-shrink: 0;
  }

  .step-content h3 {
    color: #1a365d;
    margin-bottom: 8px;
  }

  .step-content p {
    color: #4a5568;
  }

  .support-section {
    background: white;
    border-radius: 12px;
    padding: 40px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    text-align: center;
  }

  .support-section h2 {
    color: #1a365d;
    margin-bottom: 15px;
  }

  .support-section p {
    color: #4a5568;
    margin-bottom: 25px;
  }

  .support-contacts {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
  }

  .support-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    color: #3182ce;
    text-decoration: none;
    font-weight: 600;
    padding: 10px 20px;
    border: 2px solid #3182ce;
    border-radius: 6px;
    transition: all 0.3s ease;
  }

  .support-link:hover {
    background: #3182ce;
    color: white;
  }

  @media (max-width: 768px) {
    .download-card,
    .installation-steps,
    .support-section {
      padding: 25px;
    }

    .version-info {
      grid-template-columns: 1fr;
    }

    .step {
      flex-direction: column;
      text-align: center;
    }

    .support-contacts {
      flex-direction: column;
      align-items: center;
    }
  }
</style>