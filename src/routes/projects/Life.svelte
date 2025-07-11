<script lang="ts">
	import type { Component } from 'svelte';

	import PhoneFrame from '$lib/PhoneFrame.svelte';
	import lifeDesktopLightImage from '$lib/assets/life-desktop-light.png';
	import lifeMobileLightImage from '$lib/assets/life-mobile-light.png';
	import FlashIcon from '$lib/icons/FlashIcon.svelte';
	import LifeTechStackIcons from '$lib/icons/LifeTechStackIcons.svelte';
	import OfflineIcon from '$lib/icons/OfflineIcon.svelte';
	import PwaIcon from '$lib/icons/PwaIcon.svelte';
	import { CalendarClock, Goal, PocketKnife } from '@lucide/svelte';

	const features: Array<{ description: string; icon: Component; name: string }> = [
		{
			description: 'A user-friendly interface with resizable and drag-and-dropable events.',
			icon: FlashIcon,
			name: 'Highly Interactive',
		},
		{
			description:
				'Ensures offline-first data access and updates, guaranteeing uninterrupted functionality.',
			icon: OfflineIcon,
			name: 'Progressive Web App (PWA)',
		},
		{
			description: 'Empowers users to set and track goals and associate events or tasks to them.',
			icon: Goal,
			name: 'Goal Management',
		},
		{
			description:
				'Enables seamless conversion between tasks (To-Do List) and events (Calendar), offering a dynamic and adaptable planning experience.',
			icon: PocketKnife,
			name: 'Task and Event Flexibility',
		},
		{
			description: 'Supports the scheduling of recurring events.',
			icon: CalendarClock,
			name: 'Recurring Events',
		},
	];
</script>

<div class="rounded-lg border py-6 lg:py-8">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div class="mx-auto max-w-2xl lg:mx-0 lg:max-w-none">
			<p class="text-base font-semibold leading-7 text-indigo-600">Day Planner</p>
			<h1 class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Life</h1>
			<div class="mt-5 flex h-10 gap-2">
				<LifeTechStackIcons />
				<PwaIcon class="h-10 w-10 rounded-lg bg-gray-200 p-1" />
			</div>
			<p class="mt-6 text-xl leading-8 text-gray-700">
				A sophisticated, fully responsive, offline-first web application for day planning
			</p>

			<div
				class="mt-6 grid max-w-xl grid-cols-1 gap-8 text-base leading-7 text-gray-700 lg:max-w-none lg:grid-cols-2"
			>
				<p>
					Life is an elegant web app boasting a visually stunning calendar design. With its
					intuitive interface and seamless navigation, users effortlessly manage their schedules and
					tasks to reach goals faster.
				</p>
				<p>
					Developed with Svelte, showcasing proficiency with small framework ecosystems, it
					underscores my prowess in frontend development. Furthermore, it demonstrates adeptness in
					user interface design and integration of cloud services, reflecting a holistic skill set
					in crafting engaging digital experiences.
				</p>
			</div>
		</div>
	</div>

	<div class="relative overflow-hidden pt-16 lg:pt-20">
		<div class="relative mx-auto max-w-7xl px-6 lg:px-8">
			<img
				alt="screen of the app desktop"
				class="mb-[-12%] rounded-xl shadow-2xl ring-1 ring-gray-900/10"
				loading="lazy"
				src={lifeDesktopLightImage}
			/>
			<div class="right-32 top-20 sm:w-full md:absolute md:w-56 lg:w-72">
				<PhoneFrame>
					<img
						alt="screen of the app mobile"
						class="w-full"
						loading="lazy"
						src={lifeMobileLightImage}
					/>
				</PhoneFrame>
			</div>
			<div aria-hidden="true" class="relative">
				<div class="absolute -inset-x-20 bottom-0 bg-gradient-to-t from-white pt-[7%]"></div>
			</div>
		</div>
	</div>

	<div class="relative mx-auto mt-12 max-w-7xl px-6 md:mt-32 lg:px-8">
		<h2 class="text-center text-3xl font-medium tracking-tight text-gray-900">
			Some of the features
		</h2>

		<ul
			class="mx-auto mt-6 grid max-w-2xl grid-cols-1 gap-6 text-sm sm:mt-20 sm:grid-cols-2 md:gap-y-10 lg:max-w-none lg:grid-cols-3"
			role="list"
		>
			{#each features as feature (feature.name)}
				{@const Icon = feature.icon}
				<li class="rounded-2xl border border-gray-200 p-8">
					<Icon class="h-8 w-8 text-indigo-600" />
					<h3 class="mt-6 font-semibold text-gray-900">
						{feature.name}
					</h3>
					<p class="mt-2 text-gray-700">{feature.description}</p>
				</li>
			{/each}

			<li class="rounded-2xl border border-gray-200 p-8">
				<h2 class="text-2xl font-bold tracking-tight text-gray-900">Got interested?</h2>
				<p class="mb-3 mt-6">Explore the live demo and delve into the codebase on GitHub.</p>
				<div class="flex gap-3">
					<a
						class="rounded-md border border-indigo-600 bg-white px-2.5 py-1.5 text-sm font-semibold text-indigo-600 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50"
						href="https://github.com/fivaz/life"
						target="_blank"
					>
						Source code
					</a>
					<a
						class="rounded-md bg-indigo-600 px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
						href="https://life.sfivaz.com/demo"
						target="_blank"
					>
						Demo
					</a>
				</div>
			</li>
		</ul>
	</div>
</div>
