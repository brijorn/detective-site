<script>
	import Nav from '../lib/components/Nav.svelte';
	import '../app.css';
</script>

<svelte:head>
	<link rel="stylesheet" href="https://rsms.me/inter/inter.css" />
</svelte:head>

<Nav />

<slot />
<style>
	:global(body) {
		font-family: 'Inter';
	}
</style>
