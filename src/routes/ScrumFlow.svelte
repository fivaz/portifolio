<script>
	import scrumFlowImage2 from '$lib/assets/scrum-flow-2.png';
	import { Brain, ChartArea, Target, Wrench } from '@lucide/svelte';
</script>

<div class="rounded-lg border">
	<div class="relative isolate overflow-hidden px-6 py-24 sm:py-32 lg:overflow-visible lg:px-0">
		<div class="absolute inset-0 -z-10 overflow-hidden">
			<svg
				aria-hidden="true"
				class="absolute left-[max(50%,25rem)] top-0 h-[64rem] w-[128rem] -translate-x-1/2 stroke-gray-200 [mask-image:radial-gradient(64rem_64rem_at_top,white,transparent)]"
			>
				<defs>
					<pattern
						height="200"
						id="e813992c-7d03-4cc4-a2bd-151760b470a0"
						patternUnits="userSpaceOnUse"
						width="200"
						x="50%"
						y="-1"
					>
						<path d="M100 200V.5M.5 .5H200" fill="none" />
					</pattern>
				</defs>
				<svg class="overflow-visible fill-gray-50" x="50%" y="-1">
					<path
						d="M-100.5 0h201v201h-201Z M699.5 0h201v201h-201Z M499.5 400h201v201h-201Z M-300.5 600h201v201h-201Z"
						stroke-width="0"
					/>
				</svg>
				<rect
					fill="url(#e813992c-7d03-4cc4-a2bd-151760b470a0)"
					height="100%"
					stroke-width="0"
					width="100%"
				/>
			</svg>
		</div>
		<div
			class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 lg:mx-0 lg:max-w-none lg:grid-cols-2 lg:items-start lg:gap-y-10"
		>
			<div
				class="lg:col-span-2 lg:col-start-1 lg:row-start-1 lg:mx-auto lg:grid lg:w-full lg:max-w-7xl lg:grid-cols-2 lg:gap-x-8 lg:px-8"
			>
				<div class="lg:pr-4">
					<div class="lg:max-w-lg">
						<p class="text-base font-semibold leading-7 text-indigo-600">Tool for Jira</p>
						<h1 class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
							Scrum Flow
						</h1>
						<div>
							<img
								alt="tech stack"
								class="m-auto mt-5 h-10"
								loading="lazy"
								src="https://skillicons.dev/icons?i=react,ts,next,tailwind,python,postgres"
							/>
						</div>
						<p class="mt-6 text-xl leading-8 text-gray-700">
							Web application designed to enhance Scrum project management within Jira.
						</p>
					</div>
				</div>
			</div>
			<div
				class="-ml-12 -mt-12 p-12 lg:sticky lg:top-4 lg:col-start-2 lg:row-span-2 lg:row-start-1 lg:overflow-hidden"
			>
				<img
					alt="scrum flow screen"
					class="w-[48rem] max-w-none rounded-xl bg-gray-900 shadow-xl ring-1 ring-gray-400/10 sm:w-[57rem]"
					loading="lazy"
					src={scrumFlowImage2}
				/>
			</div>
			<div
				class="lg:col-span-2 lg:col-start-1 lg:row-start-2 lg:mx-auto lg:grid lg:w-full lg:max-w-7xl lg:grid-cols-2 lg:gap-x-8 lg:px-8"
			>
				<div class="lg:pr-4">
					<div class="max-w-xl text-base leading-7 text-gray-700 lg:max-w-lg">
						<ul class="mt-8 space-y-8 text-gray-600" role="list">
							<li class="flex gap-x-3">
								<Wrench class="mt-1 size-5 flex-none text-indigo-600" />
								<span>
									<strong class="font-semibold text-gray-900">No Setup.</strong>
									Seamlessly integrated with Jira Software through Atlassian OAuth, automatically handling
									data analysis without requiring additional setup or manual data migration.
								</span>
							</li>
							<li class="flex gap-x-3">
								<ChartArea class="mt-1 size-5 flex-none text-indigo-600" />
								<span>
									<strong class="font-semibold text-gray-900">Visual analysis.</strong>
									Features graphical representations illustrating the evolution of estimation maturity
									for the Scrum Team, aiding in visualizing team progress over time.
								</span>
							</li>
							<li class="flex gap-x-3">
								<Target class="mt-1 size-5 flex-none text-indigo-600" />
								<span>
									<strong class="font-semibold text-gray-900">Accuracy estimation.</strong>
									Provides insightful information on the accuracy of task estimates, proving particularly
									valuable during Sprint Retrospectives for assessing the efficacy of completed sprints.
									This facilitates informed decision-making and enhances planning within the Scrum framework.
								</span>
							</li>
							<li class="flex gap-x-3">
								<!--                                <div class="mt-1 size-5 flex-none text-indigo-600 fill-indigo-600">-->
								<!--&lt;!&ndash;                                    <CreativeThinkingIcon/>&ndash;&gt;-->
								<!--                                </div>-->
								<Brain class="mt-1 size-5 flex-none text-indigo-600" />
								<span>
									<strong class="font-semibold text-gray-900">Sprint Prediction.</strong>
									Includes a predictive module employing Machine Learning and Data Analysis to forecast
									the time required for upcoming tasks in a Sprint. This innovative feature contributes
									to proactive planning and resource management.
								</span>
							</li>
						</ul>
						<h2 class="mt-16 text-2xl font-bold tracking-tight text-gray-900">
							Interested in trying it out?
						</h2>
						<p class="mb-3 mt-6">
							Explore the detailed documentation (in French) and try out the live demo
						</p>
						<div class="flex gap-3">
							<a
								class="rounded-md border border-indigo-600 bg-white px-2.5 py-1.5 text-sm font-semibold text-indigo-600 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50"
								href="https://scrum-flow-thesis.sfivaz.com"
								target="_blank"
							>
								Documentation
							</a>
							<a
								class="rounded-md bg-indigo-600 px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
								href="https://scrum-flow.sfivaz.com/demo"
								target="_blank"
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
