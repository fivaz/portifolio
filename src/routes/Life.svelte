<script lang='ts'>
	import type { ComponentType } from 'svelte';

	import PhoneFrame from '$lib/PhoneFrame.svelte';
	import TouchIcon from '$lib/TouchIcon.svelte';
	import life3Image from '$lib/assets/life-4.png';
	import lifeMobileImage from '$lib/assets/life-mobile.png';
	import { WrenchScrewdriver } from '@steeze-ui/heroicons';
	import { AreaChart, Target, TrendingUp } from '@steeze-ui/lucide-icons';
	import { Icon } from '@steeze-ui/svelte-icon';

	const features: Array<{ description: string, icon: ComponentType, name: string }> = [
		{
			description: 'Incorporates a highly interactive interface with features such as resizable and drag-and-dropable events, facilitating a user-friendly and customizable experience',
			icon: TouchIcon,
			name: 'Highly Interactive',
		},
		{
			description: 'Ensures an offline-first approach for data access and updates, providing users with uninterrupted functionality even in offline mode.',
			icon: TouchIcon,
			name: 'Progressive Web App (PWA)',
		},
		{
			description: 'Seamlessly integrates a TODO list for effective task management within the planner.',
			icon: TouchIcon,
			name: 'TODO List Integration',
		},
		{
			description: 'Allows users to set and track goals, with the flexibility to create events or tasks attached to those goals.',
			icon: TouchIcon,
			name: 'Goal Management',
		},
		{
			description: 'Enables users to convert tasks (ToDo List) to events (Calendar) and vice-versa, offering a dynamic and adaptable planning experience.',
			icon: TouchIcon,
			name: 'Task and Event Flexibility',
		},
		{
			description: 'Supports the scheduling of recurring events, offering a comprehensive solution for repetitive activities',
			icon: TouchIcon,
			name: 'Recurring Events',
		},
	];

</script>


crafted with Svelte, Typescript, Tailwind, Firebase, and Storybook.
Technology Proficiency:
<div class='bg-white py-24 sm:py-32'>
	<div class='mx-auto max-w-7xl px-6 lg:px-8'>
		<div class='mx-auto max-w-2xl lg:mx-0 lg:max-w-none'>
			<p class='text-base font-semibold leading-7 text-indigo-600'>Day planer</p>
			<h1 class='mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl'>Life</h1>
			<img
				alt="tech stack"
				class="mt-5 h-10"
				src="https://skillicons.dev/icons?i=svelte,ts,tailwind,firebase"
			/>
			<div class='mt-10 grid max-w-xl grid-cols-1 gap-8 text-base leading-7 text-gray-700 lg:max-w-none lg:grid-cols-2'>
				<div>
					<p>
						A sophisticated Day Planner offline-first web application
					</p>

					<p class='mt-8'>Featuring an aesthetically pleasing calendar design, providing
						an intuitive and visually appealing user experience.
						Built with Svelte, showcasing my ability to excel in a framework with a growing ecosystem. This project highlights my skill in maximizing language capabilities without relying heavily on third-party libraries.
					</p>
				</div>

				<div>
					<p>
						This project exemplifies my proficiency in frontend development, user interface design, and seamless
						integration with cloud services. Leveraging modern frameworks and libraries ensures a polished and
						responsive user experience.
					</p>

					<h2 class='mt-16 text-2xl font-bold tracking-tight text-gray-900'>
						Got interested ?
					</h2>
					<p class='mb-3 mt-6'>
						Explore the live demo and delve into the codebase on GitHub.
					</p>
					<div class='flex gap-3'>
						<a
							class='rounded-md border border-indigo-600 bg-white px-2.5 py-1.5 text-sm font-semibold text-indigo-600 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50'
							href='https://github.com/fivaz/life'
							target='_blank'
						>
							Source code
						</a>
						<a
							class='rounded-md bg-indigo-600 px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600'
							href='https://life.sfivaz.com/demo'
							target='_blank'
						>
							Demo
						</a>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class='relative overflow-hidden pt-16 lg:pt-20'>
		<div class='mx-auto max-w-7xl px-6 lg:px-8 relative'>
			<img alt='screen of the app desktop' class='mb-[-12%] rounded-xl shadow-2xl ring-1 ring-gray-900/10'
					 src={life3Image}>
			<div class='w-80 absolute top-20 right-32'>
				<PhoneFrame>
					<img
						alt='screen of the app mobile'
						class='w-full'
						src={lifeMobileImage}
					/>
				</PhoneFrame>
			</div>
			<div aria-hidden='true' class='relative'>
				<div class='absolute -inset-x-20 bottom-0 bg-gradient-to-t from-white pt-[7%]'></div>
			</div>
		</div>
	</div>

	<div class='mx-auto max-w-7xl px-6 lg:px-8 relative'>
		<ul
			class='mx-auto mt-16 grid max-w-2xl grid-cols-1 gap-6 text-sm sm:mt-20 sm:grid-cols-2 md:gap-y-10 lg:max-w-none lg:grid-cols-3'
			role='list'
		>
			{#each features as feature (feature.name)}
				<li
					class='rounded-2xl border border-gray-200 p-8'
				>
					<svelte:component class='h-8 w-8' this={feature.icon} />
					<h3 class='mt-6 font-semibold text-gray-900'>
						{feature.name}
					</h3>
					<p class='mt-2 text-gray-700'>{feature.description}</p>
				</li>
			{/each}
		</ul>
	</div>


</div>