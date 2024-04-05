<script>
	import GithubIcon from '$lib/GithubIcon.svelte';
	import LinkedinIcon from '$lib/LinkedinIcon.svelte';
	import LiquidCircle from '$lib/LiquidCircle.svelte';
	import profile from '$lib/assets/profile.jpeg';

	import Navbar from './Navbar.svelte';
</script>

<Navbar />

<main class="bg-gray-50 h-screen mt-16">
	<h1>Hi, I'm Stefane Fivaz</h1>
	<h3>
		A versatile software engineer with a Bachelor of Science in Business Information Technology,
		demonstrating expertise across the entire software development lifecycle. Proficient in
		front-end and back-end technologies, with a sharp focus on user experience and a commitment to
		producing clean, maintainable code.
	</h3>
	<div class="flex">
		<LinkedinIcon />
		<GithubIcon />
	</div>
	<LiquidCircle>
		<img alt="profile" src={profile} />
	</LiquidCircle>
	<div>
		<h2>Tech Stack</h2>
		<div>
			<img
				alt="tech stack"
				src="https://skillicons.dev/icons?i=html,css,js,ts,react,svelte,vue,angular,next,python,nodejs,firebase,aws,docker"
			/>
		</div>
	</div>
</main>
