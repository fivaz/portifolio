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

<section
	class='py-20 sm:py-32'
>
	<div class='mx-auto max-w-7xl px-4 sm:px-6 lg:px-8'>
		<div class='mx-auto max-w-2xl sm:text-center'>
			<h2 class='text-3xl font-medium tracking-tight text-gray-900'>
				Now is the time to build your portfolio.
			</h2>
			<p class='mt-2 text-lg text-gray-600'>
				With typical market returns, you have to start young to secure your
				future. With Pocket, it’s never too late to build your nest egg.
			</p>
		</div>
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
</section>


<div class='bg-white py-24 sm:py-32'>
	<div class='mx-auto max-w-7xl px-6 lg:px-8'>
		<div class='mx-auto max-w-2xl lg:mx-0 lg:max-w-none'>
			<p class='text-base font-semibold leading-7 text-indigo-600'>Deploy faster</p>
			<h1 class='mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl'>A better workflow</h1>
			<div class='mt-10 grid max-w-xl grid-cols-1 gap-8 text-base leading-7 text-gray-700 lg:max-w-none lg:grid-cols-2'>

			</div>
			<div class='mt-10 flex'>
				<a
					class='rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600'
					href='#'>
					Get started
				</a>
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
</div>


<div class='m-auto rounded-lg border md:w-[880px]'>
	<div class='relative isolate overflow-hidden px-6 py-24 sm:py-32 lg:overflow-visible lg:px-0'>
		<div class='absolute inset-0 -z-10 overflow-hidden'>
			<svg
				aria-hidden='true'
				class='absolute left-[max(50%,25rem)] top-0 h-[64rem] w-[128rem] -translate-x-1/2 stroke-gray-200 [mask-image:radial-gradient(64rem_64rem_at_top,white,transparent)]'
			>
				<defs>
					<pattern
						height='200'
						id='e813992c-7d03-4cc4-a2bd-151760b470a0'
						patternUnits='userSpaceOnUse'
						width='200'
						x='50%'
						y='-1'
					>
						<path d='M100 200V.5M.5 .5H200' fill='none' />
					</pattern>
				</defs>
				<svg class='overflow-visible fill-gray-50' x='50%' y='-1'>
					<path
						d='M-100.5 0h201v201h-201Z M699.5 0h201v201h-201Z M499.5 400h201v201h-201Z M-300.5 600h201v201h-201Z'
						stroke-width='0'
					/>
				</svg>
				<rect
					fill='url(#e813992c-7d03-4cc4-a2bd-151760b470a0)'
					height='100%'
					stroke-width='0'
					width='100%'
				/>
			</svg>
		</div>
		<div
			class='mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 lg:mx-0 lg:max-w-none lg:grid-cols-2 lg:items-start lg:gap-y-10'
		>
			<div
				class='lg:col-span-2 lg:col-start-1 lg:row-start-1 lg:mx-auto lg:grid lg:w-full lg:max-w-7xl lg:grid-cols-2 lg:gap-x-8 lg:px-8'
			>
				<div class='lg:pr-4'>
					<div class='lg:max-w-lg'>
						<p class='text-base font-semibold leading-7 text-indigo-600'>Daily Planner</p>
						<h1 class='mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl'>Life</h1>
						<p class='mt-6 text-xl leading-8 text-gray-700'>
							Web application designed to enhance Scrum project management within Jira.
						</p>
						<div>
							<img
								alt='tech stack'
								class='m-auto mt-5 h-8'
								src='https://skillicons.dev/icons?i=react,ts,next,tailwind,python,postgres'
							/>
						</div>
					</div>
				</div>
			</div>
			<div
				class='relative -ml-12 -mt-12 p-12 pb-32 lg:sticky lg:top-4 lg:col-start-2 lg:row-span-2 lg:row-start-1 lg:overflow-hidden'
			>
				<img
					alt='scrum-flow screen'
					class='w-[48rem] max-w-none rounded-xl bg-gray-900 shadow-xl ring-1 ring-gray-400/10 sm:w-[57rem]'
					src={life3Image}
				/>
				<img
					alt='scrum-flow screen'
					class='absolute right-0 top-36 w-52 max-w-none rounded-xl bg-gray-900 shadow-xl ring-1 ring-gray-400/10 lg:top-48'
					src={lifeMobileImage}
				/>
			</div>
			<div
				class='lg:col-span-2 lg:col-start-1 lg:row-start-2 lg:mx-auto lg:grid lg:w-full lg:max-w-7xl lg:grid-cols-2 lg:gap-x-8 lg:px-8'
			>
				<div class='lg:pr-4'>
					<div class='max-w-xl text-base leading-7 text-gray-700 lg:max-w-lg'>
						<ul class='mt-8 space-y-8 text-gray-600' role='list'>
							<li class='flex gap-x-3'>
								<Icon class='mt-1 h-5 w-5 flex-none text-indigo-600' src={WrenchScrewdriver} />
								<span>
									<strong class='font-semibold text-gray-900'>No Setup.</strong>
									Seamlessly integrated with Jira Software through Atlassian OAuth, automatically handling
									data analysis without requiring additional setup or manual data migration.
								</span>
							</li>
							<li class='flex gap-x-3'>
								<Icon class='mt-1 h-5 w-5 flex-none text-indigo-600' src={AreaChart} />
								<span>
									<strong class='font-semibold text-gray-900'>Visual analysis.</strong>
									Features graphical representations illustrating the evolution of estimation maturity
									for the Scrum Team, aiding in visualizing team progress over time.
								</span>
							</li>
							<li class='flex gap-x-3'>
								<Icon class='mt-1 h-5 w-5 flex-none text-indigo-600' src={Target} />
								<span>
									<strong class='font-semibold text-gray-900'>Accuracy estimation.</strong>
									Provides insightful information on the accuracy of task estimates, proving particularly
									valuable during Sprint Retrospectives for assessing the efficacy of completed sprints.
									This facilitates informed decision-making and enhances planning within the Scrum framework.
								</span>
							</li>
							<li class='flex gap-x-3'>
								<Icon class='mt-1 h-5 w-5 flex-none text-indigo-600' src={TrendingUp} />
								<span>
									<strong class='font-semibold text-gray-900'>Sprint Prediction.</strong>
									Includes a predictive module employing Machine Learning and Data Analysis to forecast
									the time required for upcoming tasks in a Sprint. This innovative feature contributes
									to proactive planning and resource management.
								</span>
							</li>
						</ul>
						<h2 class='mt-16 text-2xl font-bold tracking-tight text-gray-900'>Got interested ?</h2>
						<p class='mb-3 mt-6'>
							Explore the detailed documentation (in French) and try out the live demo
						</p>
						<div class='flex gap-3'>
							<a
								class='rounded-md border border-indigo-600 bg-white px-2.5 py-1.5 text-sm font-semibold text-indigo-600 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50'
								href='https://scrum-flow-thesis.sfivaz.com'
								target='_blank'
							>
								Documentation
							</a>
							<a
								class='rounded-md bg-indigo-600 px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600'
								href='https://scrum-flow.sfivaz.com/demo'
								target='_blank'
							>
								Demo
							</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
