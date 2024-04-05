<script>
	import Button from '$lib/Button.svelte';
	import scrumFlowImage1 from '$lib/assets/scrum-flow-1.png';
	import scrumFlowImage2 from '$lib/assets/scrum-flow-2.png';
</script>

<section class="p-5 h-96 bg-white w-full flex justify-center">
	<div class="md:w-[880px] flex flex-col items-center">
		<h1 class="text-3xl font-bold text-center my-5">Projects</h1>

		<div class="flex gap-5 flex-col md:flex-row items-start">
			<div>
				<img
					alt="scrum-flow page 1"
					class="rounded-lg hidden md:block w-96"
					src={scrumFlowImage1}
				/>
				<img alt="scrum-flow page 2" class="rounded-lg w-96" src={scrumFlowImage2} />
			</div>
			<div>
				<h2 class="text-2xl font-semibold mb-2">Scrum Flow</h2>
				<p>Web application designed to enhance Scrum project management within Jira</p>
				<ul class="list-disc">
					<li>Seamlessly integrated with Jira Software through Atlassian OAuth.</li>
					<li>
						Features graphical representations illustrating the evolution of estimation maturity for
						the Scrum Team, aiding in visualizing team progress over time.
					</li>
					<li>
						Provides insightful information on the accuracy of task estimates, proving particularly
						valuable during Sprint Retrospectives for assessing the efficacy of completed sprints.
						This facilitates informed decision-making and enhances planning within the Scrum
						framework.
					</li>
					<li>
						Includes a predictive module employing Machine Learning and Data Analysis to forecast
						the time required for upcoming tasks in a Sprint. This innovative feature contributes to
						proactive planning and resource management.
					</li>
				</ul>
				<div class="flex justify-center gap-5 p-5">
					<a href="https://scrum-flow-thesis.sfivaz.com" target="_blank">
						<Button>Documentation</Button>
					</a>
					<a href="https://scrum-flow.sfivaz.com/demo" target="_blank">
						<Button>Demo</Button>
					</a>
				</div>
			</div>
		</div>

		<div></div>

		<div></div>
	</div>
</section>
