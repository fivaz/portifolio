<script>
	import GithubIcon from '$lib/GithubIcon.svelte';
	import Highlight from '$lib/Highlight.svelte';
	import LinkedinIcon from '$lib/LinkedinIcon.svelte';
	import LiquidAvatar from '$lib/LiquidImage.svelte';
</script>

<section class="flex flex-col items-center gap-5 bg-gray-50 p-5 md:w-[880px] md:justify-center scroll-mt-16" id='home'>
	<div class="flex flex-col items-center gap-5 md:flex-row-reverse">
		<div class="max-w-80">
			<LiquidAvatar />
		</div>

		<div class="flex flex-col items-center gap-5">
			<h1 class="text-center text-5xl font-bold">
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
				<Highlight>
					<a href="https://github.com/fivaz" target="_blank">
						<GithubIcon />
					</a>
				</Highlight>
				<Highlight>
					<a href="https://www.linkedin.com/in/stefane-fivaz-b3898211a" target="_blank">
						<LinkedinIcon />
					</a>
				</Highlight>
			</div>
		</div>
	</div>

	<div class="flex flex-col items-center gap-3">
		<h2 class="text-lg font-semibold">Tech Stack</h2>
		<div class="flex flex-col items-center gap-3 md:gap-2 lg:flex-row">
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

<style>
	@media (min-width: 768px) {
		section {
			/*64px is the height of the navbar*/
			height: calc(100vh - 64px);
		}
	}
</style>
