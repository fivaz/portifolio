<script>
	import Highlight from '$lib/Highlight.svelte';
	import LiquidAvatar from '$lib/LiquidAvatar.svelte';
	import GithubIcon from '$lib/icons/GithubIcon.svelte';
	import LinkedinIcon from '$lib/icons/LinkedinIcon.svelte';
	import { ArrowDown } from '@lucide/svelte';
</script>

<section
	class="relative flex scroll-mt-16 flex-col items-center gap-5 bg-gray-50 p-5 md:w-[768px] md:justify-center lg:w-[880px]"
	id="home"
>
	<div class="flex flex-col items-center gap-5 md:flex-row-reverse">
		<LiquidAvatar />

		<div class="flex flex-col items-center gap-5">
			<h1 class="text-center text-5xl font-bold">
				Hi, I'm <Highlight>Stefane Fivaz</Highlight>
				👋
			</h1>

			<p>
				A versatile software engineer with a
				<Highlight>Bachelor of Science in Business IT</Highlight>,
				<Highlight>over 1.5 years of professional experience</Highlight> in a company setting, and <Highlight
					>more than 10 years of hands-on coding practice</Highlight
				>. Proficient in <Highlight>front-end</Highlight> and <Highlight>back-end</Highlight> technologies,
				with a sharp focus on <Highlight>user experience</Highlight> and a commitment to producing
				<Highlight>clean</Highlight>, <Highlight>maintainable code</Highlight>.
			</p>

			<div class="flex gap-3">
				<Highlight>
					<a href="https://github.com/fivaz" target="_blank">
						<GithubIcon />
					</a>
				</Highlight>
				<Highlight>
					<a href="https://www.linkedin.com/in/stefanefivaz" target="_blank">
						<LinkedinIcon />
					</a>
				</Highlight>
			</div>
		</div>
	</div>

	<div class="flex flex-col items-center gap-3">
		<h2 class="text-lg font-semibold">Tech Stack</h2>
		<div class="grid grid-cols-1 gap-2 md:grid-cols-2 lg:grid-cols-4">
			<img alt="tech stack" src="https://skillicons.dev/icons?i=html,css,js,ts" />
			<img alt="tech stack" src="https://skillicons.dev/icons?i=react,svelte,vue,angular" />
			<img alt="tech stack" src="https://skillicons.dev/icons?i=nodejs,python,php,firebase" />
			<img alt="tech stack" src="https://skillicons.dev/icons?i=mongodb,postgres,aws,docker" />
		</div>
	</div>

	<a
		class="border-1 absolute bottom-4 hidden size-10 animate-bounce items-center rounded-full border-indigo-600 bg-white p-2 text-indigo-600 shadow-lg ring-1 ring-slate-900/5 hover:bg-indigo-500 hover:text-white focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 md:flex"
		href="#projects"
	>
		<ArrowDown class="size-10" />
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
