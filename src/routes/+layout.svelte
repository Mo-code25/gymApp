<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
	import "../app.css";
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}

<Footer/>


