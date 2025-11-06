<script>
	import favicon from '$lib/assets/favicon.png';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>
<header style="display:flex; align-items:center; justify-content:end; padding:1rem; background:linear-gradient(120deg, #3182ce, #74b9ff);">
	<img style="height: 40px; margin-right: 1rem;" src="images/favicon.png" alt="logo" srcset="">
	<h1 class="logo">Space4</h1>
</header>
<style>
	@media (max-width: 768px){.logo{display: none;}}	
</style>

{@render children()}