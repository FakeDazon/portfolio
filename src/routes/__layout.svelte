<script>
	import Footer from '$lib/components/footer.svelte';
	import Navbar from '$lib/components/navbar.svelte';
	import { onMount } from 'svelte';
	import '$lib/styles/app.css';
	import '$lib/styles/font.css';
	let y;
</script>

<svelte:window bind:innerWidth={y} />
<main>
	<Navbar width={y} />
	<slot />
	<Footer />
</main>
