<script>
	import favicon from '$lib/assets/favicon.png';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>
<header style="display:flex; align-items:center; justify-content:end; padding:1rem; background:#f8f8f8;">
	<img style="height: 40px; margin-right: 1rem;" src="images/favicon.png" alt="logo" srcset="">
	<h1 class="logo">Space4</h1>
</header>
<style>
	@media (max-width: 768){
		.logo{
			width: 100px;
		}
	}

	@media (max-width: 480){
		.logo{
			width: 70px;
		}
	}
	
</style>

{@render children()}