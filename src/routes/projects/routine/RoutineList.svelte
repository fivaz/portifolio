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
	import ReactIcon from '$lib/icons/ReactIcon.svelte';
	import JavaIcon from '$lib/icons/JavaIcon.svelte';
	import TypescriptIcon from '$lib/icons/TypescriptIcon.svelte';
	import SpringIcon from '$lib/icons/SpringIcon.svelte';
	import FirebaseIcon from '$lib/icons/FirebaseIcon.svelte';
	import GeminiIcon from '$lib/icons/GeminiIcon.svelte';
	import SentryIcon from '$lib/icons/SentryIcon.svelte';
	import DockerIcon from '$lib/icons/DockerIcon.svelte';
	import SwaggerIcon from '$lib/icons/SwaggerIcon.svelte';
	import GitHubActionsIcon from '$lib/icons/GitHubActionsIcon.svelte';
	import RecraftIcon from '$lib/icons/RecraftIcon.svelte';

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
			icon: ReactIcon,
			name: 'React',
		},
		{
			icon: JavaIcon,
			name: 'Java',
		},
		{
			icon: TypescriptIcon,
			name: 'Typescript',
		},
		{
			icon: SpringIcon,
			name: 'Spring Boot',
		},
		{
			icon: FirebaseIcon,
			name: 'Firebase',
		},
		{
			icon: GeminiIcon,
			name: 'Gemini API',
		},
		{
			icon: RecraftIcon,
			name: 'Recraft AI',
		},
		{
			icon: SentryIcon,
			name: 'Sentry',
		},
		{
			icon: DockerIcon,
			name: 'Docker',
		},
		{
			icon: GitHubActionsIcon,
			name: 'GitHub Actions',
		},
		{
			icon: SwaggerIcon,
			name: 'Swagger UI',
		},
	];
</script>

{#snippet title(text: string)}
	<h2 class="text-2xl font-bold tracking-tight text-gray-900">{text}</h2>
{/snippet}

<div class="flex flex-col gap-8">
	{@render title('Key Technologies:')}

	<ul class="flex flex-wrap gap-1">
		{#each technologies as technology}
			{@const Icon = technology.icon}
			<li class="flex items-center gap-3 rounded-lg border-2 border-indigo-500 px-3 py-2">
				<Icon class="size-8" />
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
