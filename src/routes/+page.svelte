<script>
	import HomeSection from './HomeSection.svelte';
	import Navbar from './Navbar.svelte';
	import Resume from './Resume.svelte';
	import Projects from './projects/Projects.svelte';
</script>

<div class="relative">
	<Navbar />
	<main class="flex flex-col items-center bg-gray-50 pt-16">
		<HomeSection />

		<Projects />

		<Resume />
	</main>
</div>
