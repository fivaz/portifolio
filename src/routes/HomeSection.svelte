<script>
	import GithubIcon from '$lib/GithubIcon.svelte';
	import Highlight from '$lib/Highlight.svelte';
	import LinkedinIcon from '$lib/LinkedinIcon.svelte';
	import LiquidAvatar from '$lib/LiquidImage.svelte';
	import { ArrowDown } from '@steeze-ui/heroicons';
	import { Icon } from '@steeze-ui/svelte-icon';
</script>

<section
	class="relative flex scroll-mt-16 flex-col items-center gap-5 bg-gray-50 p-5 md:w-[880px] md:justify-center"
	id="home"
>
	<div class="flex flex-col items-center gap-5 md:flex-row-reverse">
		<LiquidAvatar />

		<div class="flex flex-col items-center gap-5">
			<h1 class="text-center text-5xl font-bold">
				Hi, I'm
				<Highlight>Stefane Fivaz</Highlight>
				👋
			</h1>

			<p>
				Versatile software engineer with a BS in Business IT and more than 7 years with development,
				demonstrating expertise across the entire software development lifecycle, with a sharp focus
				on user experience and a commitment to producing clean, maintainable code.
			</p>

			<h3>
				A versatile software engineer proficient in front-end and back-end technologies, with a
				sharp focus on user experience and a commitment to producing clean, maintainable code.
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
			<img alt="tech stack" src="https://skillicons.dev/icons?i=svelte,vue,angular,nodejs,python" />
			<img
				alt="tech stack"
				src="https://skillicons.dev/icons?i=firebase,aws,mongodb,postgres,docker"
			/>
		</div>
	</div>

	<a
		class="border-1 absolute bottom-4 hidden h-10 w-10 animate-bounce items-center rounded-full border-indigo-600 bg-white p-2 text-indigo-600 shadow-lg ring-1 ring-slate-900/5 hover:bg-indigo-500 hover:text-white focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 md:flex"
		href="#projects"
	>
		<Icon class="h-10 w-10" src={ArrowDown} />
	</a>
</section>

<style>
	@media (min-width: 768px) {
		section {
			/*64px is the height of the navbar*/
			height: calc(100vh - 64px);
		}
	}
</style>
