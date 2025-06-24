<script lang="ts">
	import SmallPhoneFrame from '$lib/SmallPhoneFrame.svelte';
	import routineImage2 from '$lib/assets/routine-2.png';
	import routineDiagram from '$lib/assets/routine-diagram.png';
	import LifeTechStackIcons from '$lib/icons/LifeTechStackIcons.svelte';
	import PwaIcon from '$lib/icons/PwaIcon.svelte';
</script>

<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
	<div class="flex justify-between">
		<div>
			<p class="text-base font-semibold leading-7 text-indigo-600">Turn Habits into Flow</p>
			<h1 class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
				RoutineMaster
			</h1>
			<div class="mt-5 flex h-10 gap-2">
				<LifeTechStackIcons />
				<PwaIcon class="h-10 w-10 rounded-lg bg-gray-200 p-1" />
			</div>

			<p class="mt-6 text-xl leading-8 text-gray-700">
				A productivity mobile web app that helps users build focus-driven routines with countdowns,
				real-time progress tracking, and AI-generated visuals
			</p>

			<h2>Key Technologies:</h2>
			<p>React (TypeScript), Java (Spring Boot), Firebase, Gemini API, Recraft AI</p>
			<p>Sentry, Docker, GitHub Actions, Swagger UI</p>
			<h2>Core Features (use icons for each):</h2>
			<p>⏱️ Countdown per task</p>
			<p>🔁 Real-time updates (Firestore listeners)</p>
			<p>🎨 AI-generated task visuals</p>
			<p>📈 Performance graphs</p>
			<p>🛠️ CI/CD with GitHub Actions & Docker</p>
			<p>🧪 Error monitoring with Sentry</p>
			<img alt="diagram" src={routineDiagram} />
		</div>
		<div></div>

		<SmallPhoneFrame image={routineImage2} />
	</div>
</div>
