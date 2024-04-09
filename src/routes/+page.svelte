<script>
	import HomeSection from './HomeSection.svelte';
	import Navbar from './Navbar.svelte';
	import ProjectsSection from './ProjectsSection.svelte';
</script>

<div class="relative">
	<Navbar />
	<main class="flex flex-col items-center bg-gray-50 pt-16" id='home'>
		<HomeSection />

		<ProjectsSection />

		<section class='h-96' id='resume'></section>
	</main>
</div>
