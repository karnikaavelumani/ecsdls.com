<script>
	import Nav from '$lib/components/nav/nav.svelte';
	import Footer from '$lib/components/footer/footer.svelte';
</script>

<Nav />

<slot />

<Footer />

<style>
	:global(body) {
		margin: 0;
		display: grid;
	}
</style>
