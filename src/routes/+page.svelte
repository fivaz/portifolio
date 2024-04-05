<script>
	import GithubIcon from '$lib/GithubIcon.svelte';
	import Highlight from '$lib/Highlight.svelte';
	import LinkedinIcon from '$lib/LinkedinIcon.svelte';
	import LiquidAvatar from '$lib/LiquidImage.svelte';

	import Navbar from './Navbar.svelte';
</script>

<Navbar />

<main class="bg-gray-50 flex flex-col items-center">
	<section
		class="p-5 flex flex-col gap-5 items-center bg-gray-50 md:w-[850px] h-screen md:justify-center"
	>
		<div class="flex gap-5 flex-col md:flex-row-reverse items-center">
			<div class="max-w-80">
				<LiquidAvatar />
			</div>

			<div class="flex flex-col gap-5 items-center">
				<h1 class="text-5xl text-center font-bold">
					Hi, I'm <Highlight>Stefane Fivaz</Highlight> 👋
				</h1>

				<h3>
					A versatile software engineer proficient in
					<Highlight>front-end</Highlight>
					and
					<Highlight>back-end</Highlight>
					technologies, with a sharp focus on
					<Highlight>user experience</Highlight>
					and a commitment to producing
					<Highlight>clean, maintainable code.</Highlight>
				</h3>

				<div class="flex gap-3">
					<LinkedinIcon />
					<GithubIcon />
				</div>
			</div>
		</div>

		<div class="flex flex-col items-center gap-3">
			<h2 class="text-lg font-semibold">Tech Stack</h2>
			<div class="flex flex-col lg:flex-row gap-3 md:gap-2 items-center">
				<img alt="tech stack" src="https://skillicons.dev/icons?i=html,css,js,ts,react" />
				<img
					alt="tech stack"
					src="https://skillicons.dev/icons?i=svelte,vue,angular,tailwind,python"
				/>
				<img
					alt="tech stack"
					src="https://skillicons.dev/icons?i=nodejs,firebase,aws,mongodb,postgres"
				/>
			</div>
		</div>
	</section>

	<section class="h-96 bg-white"></section>
</main>
