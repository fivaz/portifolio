<script lang="ts">
	import routineDiagram from '$lib/assets/routine-diagram.png';
	import {
		ActivityIcon,
		BrainCircuitIcon,
		ChartSplineIcon,
		LucideWorkflow,
		RefreshCw,
		RefreshCwIcon,
		Timer,
		TimerIcon,
		WorkflowIcon,
	} from '@lucide/svelte';
	import GithubActionsIcon from './GithubActionsIcon.svelte';

	const features = [
		{
			icon: TimerIcon,
			description: 'Countdown per task',
		},
		{
			icon: RefreshCwIcon,
			description: 'Real-time updates (Firestore listeners)',
		},
		{
			icon: BrainCircuitIcon,
			description: 'AI-generated task visuals',
		},
		{
			icon: ChartSplineIcon,
			description: 'Performance graphs',
		},
		{
			icon: LucideWorkflow,
			description: 'CI/CD with GitHub Actions & Docker',
		},
		{
			icon: ActivityIcon,
			description: 'Error monitoring with Sentry',
		},
	];

	const technologies = [
		{
			icon: WorkflowIcon,
			name: 'React',
		},
		{
			icon: WorkflowIcon,
			name: 'Java',
		},
		{
			icon: WorkflowIcon,
			name: 'React',
		},
		{
			icon: WorkflowIcon,
			name: 'Spring Boot',
		},
		{
			icon: WorkflowIcon,
			name: 'Firebase',
		},
		{
			icon: WorkflowIcon,
			name: 'Gemini API',
		},
		{
			icon: WorkflowIcon,
			name: 'Recraft AI',
		},
		{
			icon: WorkflowIcon,
			name: 'Sentry',
		},
		{
			icon: WorkflowIcon,
			name: 'Docker',
		},
		{
			icon: WorkflowIcon,
			name: 'GitHub Actions',
		},
		{
			icon: WorkflowIcon,
			name: 'Swagger UI',
		},
	];
</script>

{#snippet title(text: string)}
	<h2 class="text-2xl font-bold tracking-tight text-gray-900">{text}</h2>
{/snippet}

<div class="flex flex-col gap-8">
	{@render title('Key Technologies:')}

	<ul>
		{#each technologies as technology}
			{@const Icon = technology.icon}
			<li class="flex gap-x-3">
				<Icon class="size-5 text-indigo-600" />
				<span>{technology.name}</span>
			</li>
		{/each}
	</ul>

	{@render title('Core Features:')}

	<ul>
		{#each features as feature}
			{@const Icon = feature.icon}
			<li class="flex gap-x-3">
				<Icon class="size-5 text-indigo-600" />
				<span>{feature.description}</span>
			</li>
		{/each}
	</ul>

	{@render title('How I built it:')}

	<img src={routineDiagram} alt="diagram" />
</div>
