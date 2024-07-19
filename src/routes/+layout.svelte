<script>
	import '../app.css';
	import 'aos/dist/aos.css';
	import AOS from 'aos';
	import { onMount } from 'svelte';
	onMount(() => {
		AOS.init();
	});
</script>

<main class="bg-[#f2f2e9] overflow-hidden">
	<slot />
</main>

<style>
</style>


