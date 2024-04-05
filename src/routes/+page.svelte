<script>
	import Button from '$lib/Button.svelte';
	import GithubIcon from '$lib/GithubIcon.svelte';
	import Highlight from '$lib/Highlight.svelte';
	import LinkedinIcon from '$lib/LinkedinIcon.svelte';
	import LiquidAvatar from '$lib/LiquidImage.svelte';
	import scrumFlowImage1 from '$lib/assets/scrum-flow-1.png';
	import scrumFlowImage2 from '$lib/assets/scrum-flow-2.png';

	import HomeSection from './HomeSection.svelte';
	import Navbar from './Navbar.svelte';
	import ProjectsSection from './ProjectsSection.svelte';
</script>

<div class="relative">
	<Navbar />
	<main class="pt-16 bg-gray-50 flex flex-col items-center">
		<HomeSection />

		<ProjectsSection />
	</main>
</div>
