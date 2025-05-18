<script lang="ts">
	import { Brain, ChartArea, Target, Wrench } from '@lucide/svelte';
</script>

<ul class="mt-8 space-y-8 text-gray-600" role="list">
	<li class="flex gap-x-3">
		<Wrench class="mt-1 size-5 flex-none text-indigo-600" />
		<span>
			<strong class="font-semibold text-gray-900">No Setup.</strong>
			Seamlessly integrated with Jira Software through Atlassian OAuth, automatically handling data analysis
			without requiring additional setup or manual data migration.
		</span>
	</li>
	<li class="flex gap-x-3">
		<ChartArea class="mt-1 size-5 flex-none text-indigo-600" />
		<span>
			<strong class="font-semibold text-gray-900">Visual analysis.</strong>
			Features graphical representations illustrating the evolution of estimation maturity for the Scrum
			Team, aiding in visualizing team progress over time.
		</span>
	</li>
	<li class="flex gap-x-3">
		<Target class="mt-1 size-5 flex-none text-indigo-600" />
		<span>
			<strong class="font-semibold text-gray-900">Accuracy estimation.</strong>
			Provides insightful information on the accuracy of task estimates, proving particularly valuable
			during Sprint Retrospectives for assessing the efficacy of completed sprints. This facilitates
			informed decision-making and enhances planning within the Scrum framework.
		</span>
	</li>
	<li class="flex gap-x-3">
		<!--                                <div class="mt-1 size-5 flex-none text-indigo-600 fill-indigo-600">-->
		<!--&lt;!&ndash;                                    <CreativeThinkingIcon/>&ndash;&gt;-->
		<!--                                </div>-->
		<Brain class="mt-1 size-5 flex-none text-indigo-600" />
		<span>
			<strong class="font-semibold text-gray-900">Sprint Prediction.</strong>
			Includes a predictive module employing Machine Learning and Data Analysis to forecast the time
			required for upcoming tasks in a Sprint. This innovative feature contributes to proactive planning
			and resource management.
		</span>
	</li>
</ul>
