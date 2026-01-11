<script>
  let features = [
    {
      title: "ثبت دقیق داده‌ها",
      description: "ثبت خودکار و دقیق تمامی داده‌های تانک تیل با دقت بالا",
      icon: "📊"
    },
    {
      title: "آنالیز پیشرفته",
      description: "تحلیل داده‌ها با الگوریتم‌های هوشمند و ارائه گزارش‌های تحلیلی",
      icon: "🔍"
    },
    {
      title: "پشتیبانی از فرمت‌های مختلف",
      description: "قابلیت کار با داده‌های ورودی در فرمت‌های مختلف و خروجی قابل تنظیم",
      icon: "📁"
    },
    {
      title: "داشبورد مدیریتی",
      description: "نمایش گرافیکی و تعاملی داده‌ها برای تصمیم‌گیری بهتر",
      icon: "📈"
    },
    {
      title: "امنیت بالا",
      description: "حفظ امنیت و محرمانگی داده‌ها با سیستم رمزنگاری پیشرفته",
      icon: "🔒"
    },
    {
      title: "پشتیبانی 24/7",
      description: "پشتیبانی فنی دائمی برای رفع مشکلات و پاسخ به سوالات",
      icon: "🛠️"
    }
  ];

  let systemRequirements = [
    "سیستم عامل: ویندوز 10، 11  ",
    "پردازنده: Intel Core i5 یا معادل آن",
    "حافظه رم: حداقل 4 گیگابایت",
    "فضای ذخیره‌سازی: 256 مگابایت فضای آزاد",
    "اتصال اینترنت برای فعال‌سازی و بروزرسانی"
  ];
</script>

<svelte:head>
  <title>نرم‌افزار ثبت و آنالیز داده‌های تانک تیل</title>
  <meta name="description" content="نرم‌افزار پیشرفته ثبت و آنالیز داده‌های تانک تیل با قابلیت‌های فوق‌العاده" />
</svelte:head>

<div class="container">
  <!-- بخش هدر و معرفی -->
  <header class="hero">
    <div class="hero-content">
      <h1 class="hero-title">نرم‌افزار ثبت و آنالیز داده‌های تانک تیل</h1>
      <p class="hero-description">
        راه‌حلی جامع و پیشرفته برای مدیریت، ثبت و تحلیل داده‌های تانک تیل با دقت و سرعت بالا
      </p>
      <div class="hero-buttons">
        <a href="/download" class="btn btn-primary">دانلود نرم‌افزار</a>
        <a href="#features" class="btn btn-secondary">مشاهده قابلیت‌ها</a>
      </div>
    </div>
    <div class="hero-image">
      <div class="software-preview">
        <div class="preview-window">
          <div class="preview-header">
            <div class="window-controls">
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>
          <div class="preview-content">
            <div class="data-chart"></div>
            <div class="data-table">
              <div class="table-row header">
                <div>زمان</div>
                <div>دما</div>
                <div>فشار</div>
                <div>حجم</div>
              </div>
              <div class="table-row">
                <div>10:30</div>
                <div>45°C</div>
                <div>2.5 bar</div>
                <div>85%</div>
              </div>
              <div class="table-row">
                <div>10:35</div>
                <div>46°C</div>
                <div>2.6 bar</div>
                <div>84%</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>

  <!-- بخش ویژگی‌ها -->
  <section id="features" class="features-section">
    <h2 class="section-title">قابلیت‌های نرم‌افزار</h2>
    <div class="features-grid">
      {#each features as feature}
        <div class="feature-card">
          <div class="feature-icon">{feature.icon}</div>
          <h3 class="feature-title">{feature.title}</h3>
          <p class="feature-description">{feature.description}</p>
        </div>
      {/each}
    </div>
  </section>
      <section class="tutorials-section">
        <div class="tutorials-container">
             <div class="tutorials-cta">
                <div class="cta-content">
                    <div class="cta-icon">🎓</div>
                    <h2>آموزش رایگان نرم‌افزار</h2>
                    <p>ویدئوهای آموزشی تخصصی برای تسلط کامل بر نرم‌افزار</p>
                    <a class="cta-button" href="https://whatsapp.com/channel/0029Vb6SYTr5Ejy17hkLHb2C">
                 
                          ثبت‌نام رایگان
                          <span class="arrow">→</span>
                      
                  </a>
                </div>
            </div>
        </div>
    </section>
  <!-- بخش سیستم مورد نیاز -->
  <section class="requirements-section">
    <h2 class="section-title">سیستم مورد نیاز</h2>
    <div class="requirements-list">
      {#each systemRequirements as requirement}
        <div class="requirement-item">
          <span class="checkmark">✓</span>
          <span>{requirement}</span>
        </div>
      {/each}
    </div>
  </section>

  <!-- بخش دانلود -->
  <section class="download-section">
    <div class="download-content">
      <h2 class="section-title">همین حالا نرم‌افزار را دانلود کنید</h2>
      <p>نسخه کامل نرم‌افزار با تمامی قابلیت‌ها - رایگان برای 2 روز اول</p>
      <a href="/download" class="btn btn-primary btn-large">دانلود نسخه 1.6.0</a>
      <div class="download-info">
        <span>حجم: 106 مگابایت</span>
        <span>•</span>
        <span>آخرین بروزرسانی: 1404/8/22</span>
      </div>
      <footer>
        <p style="font-size:smaller;">© 2024 تیم برنامه نویسی Space4 بلخاب<br> تمام حقوق محفوظ است</p>
      </footer>     </div>
  </section>
</div>

<style>
  :global(*) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  :global(body) {
    background-color: #f8f9fa;
    color: #333;
    line-height: 1.6;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }

  /* استایل هدر */
  .hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 80px 0;
    gap: 40px;
  }

  .hero-content {
    flex: 1;
  }

  .hero-title {
    font-size: 2.5rem;
    color: #1a365d;
    margin-bottom: 20px;
    line-height: 1.2;
  }

  .hero-description {
    font-size: 1.2rem;
    color: #4a5568;
    margin-bottom: 30px;
    max-width: 500px;
  }

  .hero-buttons {
    display: flex;
    gap: 15px;
  }

  .btn {
    display: inline-block;
    padding: 12px 24px;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
  }

  .btn-primary {
    background-color: #3182ce;
    color: white;
  }

  .btn-primary:hover {
    background-color: #2c5aa0;
  }

  .btn-secondary {
    background-color: transparent;
    color: #3182ce;
    border: 2px solid #3182ce;
  }

  .btn-secondary:hover {
    background-color: #3182ce;
    color: white;
  }

  .btn-large {
    padding: 15px 30px;
    font-size: 1.1rem;
  }

  /* استایل پیش‌نمایش نرم‌افزار */
  .software-preview {
    flex: 1;
    display: flex;
    justify-content: center;
  }

  .preview-window {
    width: 100%;
    max-width: 500px;
    background: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
  }

  .preview-header {
    background: #2d3748;
    padding: 10px 15px;
  }

  .window-controls {
    display: flex;
    gap: 8px;
  }

  .window-controls span {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: #e53e3e;
  }

  .window-controls span:nth-child(2) {
    background: #ecc94b;
  }

  .window-controls span:nth-child(3) {
    background: #48bb78;
  }

  .preview-content {
    padding: 20px;
  }

  .data-chart {
    height: 150px;
    background: linear-gradient(120deg, #a0c4ff, #74b9ff);
    border-radius: 4px;
    margin-bottom: 20px;
    position: relative;
  }

  .data-chart::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      linear-gradient(90deg, transparent 49%, rgba(255,255,255,0.3) 50%, transparent 51%),
      linear-gradient(transparent 49%, rgba(255,255,255,0.3) 50%, transparent 51%);
    background-size: 20px 20px;
  }

  .data-table {
    width: 100%;
  }

  .table-row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    padding: 8px 0;
    border-bottom: 1px solid #e2e8f0;
  }

  .table-row.header {
    font-weight: bold;
    background-color: #f7fafc;
  }

  /* استایل بخش ویژگی‌ها */
  .section-title {
    text-align: center;
    font-size: 2rem;
    color: #1a365d;
    margin-bottom: 50px;
  }

  .features-section {
    padding: 80px 0;
    background-color: white;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
  }

  .feature-card {
    background: #f8f9fa;
    border-radius: 8px;
    padding: 30px;
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .feature-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .feature-icon {
    font-size: 3rem;
    margin-bottom: 20px;
  }

  .feature-title {
    font-size: 1.3rem;
    color: #2d3748;
    margin-bottom: 15px;
  }

  .feature-description {
    color: #4a5568;
  }
      /* استایل‌های بخش آموزش */
    .tutorials-section {
        margin: 6rem 0;
        padding: 3rem 0;
        color: #fff;
        background: rgba(255, 255, 255, 0.05);
        border-radius: 25px;
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }


    .tutorials-container {
        max-width: 1100px;
        margin: 0 auto;
        padding: 0 2rem;
    }
  
    .tutorials-cta {
        background: linear-gradient(135deg, #72b7fd 0%, #1867b0 100%);
        border-radius: 20px;
        padding: 3rem 2rem;
        text-align: center;
        position: relative;
        overflow: hidden;
    }

    .tutorials-cta::before {
        content: '';
        position: absolute;
        top: -50%;
        left: -50%;
        width: 200%;
        height: 200%;
        background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
        animation: rotate 10s linear infinite;
    }

    .cta-content {
        position: relative;
        z-index: 2;
    }

    .cta-icon {
        font-size: 4rem;
        margin-bottom: 1rem;
        animation: float 3s ease-in-out infinite;
    }

    .cta-content h2 {
        font-size: 1.8rem;
        margin-bottom: 1rem;
    }

    .cta-content p {
        font-size: 1.1rem;
        opacity: 0.9;
        margin-bottom: 2rem;
        max-width: 500px;
        margin-left: auto;
        margin-right: auto;
    }

    .cta-button {
        background: white;
        color: #667eea;
        border: none;
        padding: 1rem 2rem;
        border-radius: 25px;
        font-size: 1.1rem;
        font-weight: bold;
        cursor: pointer;
        transition: all 0.3s ease;
        display: flex;
        align-items: center;
        gap: 0.5rem;
        margin: 0 auto;
    }

    .cta-button:hover {
        transform: translateY(-3px);
        box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }

    .arrow {
        transition: transform 0.3s ease;
    }

    .cta-button:hover .arrow {
        transform: translateX(5px);
    }

       footer {
        text-align: center;
        margin-top: 4rem;
        padding-top: 2rem;
        border-top: 1px solid rgba(255,255,255,0.3);
    }
    @keyframes float {
        0%, 100% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-10px);
        }
    }

    @keyframes rotate {
        from {
            transform: rotate(0deg);
        }
        to {
            transform: rotate(360deg);
        }
    }

    @media (max-width: 768px) {
        .container {
            padding: 1rem;
        }
        
        h1 {
            font-size: 2rem;
        }
        
        .discount-card {
            width: 300px;
            height: 220px;
        }
        
        .tutorials-grid {
            grid-template-columns: 1fr;
        }
        
        .tutorial-meta {
            flex-direction: column;
            gap: 0.5rem;
        }
    }
  /* استایل بخش سیستم مورد نیاز */
  .requirements-section {
    padding: 80px 0;
  }

  .requirements-list {
    max-width: 600px;
    margin: 0 auto;
  }

  .requirement-item {
    display: flex;
    align-items: center;
    padding: 12px 0;
    border-bottom: 1px solid #e2e8f0;
  }

  .checkmark {
    color: #48bb78;
    margin-left: 10px;
    font-weight: bold;
  }

  /* استایل بخش دانلود */
  .download-section {
    padding: 80px 0;
    background-color: #1a365d;
    color: white;
    text-align: center;
  }

  .download-content {
    max-width: 600px;
    margin: 0 auto;
  }

  .download-section .section-title {
    color: white;
  }

  .download-section p {
    margin-bottom: 30px;
    font-size: 1.1rem;
  }

  .download-info {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    gap: 10px;
    color: #cbd5e0;
  }
  footer {
        text-align: center;
        margin-top: 4rem;
        padding-top: 2rem;
        border-top: 1px solid rgba(255,255,255,0.3);
    }
  /* رسپانسیو */
  @media (max-width: 768px) {
    .hero {
      flex-direction: column;
      text-align: center;
      padding: 50px 0;
    }

    .hero-buttons {
      justify-content: center;
    }

    .hero-title {
      font-size: 2rem;
    }

    .features-grid {
      grid-template-columns: 1fr;
    }
  }
</style>
