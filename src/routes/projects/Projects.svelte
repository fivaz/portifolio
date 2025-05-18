<script lang="ts">
	import Life from './Life.svelte';
	import ScrumFlow from './scrum-flow/ScrumFlow.svelte';
	import Routine from './routine/Routine.svelte';
</script>

<!--scroll-mt-16 makes the anchor div appear slight under the viewport so it's not covered by the fixed navbar -->

<section class=" w-full scroll-mt-16 bg-white" id="projects">
	<div class="mx-auto flex max-w-7xl flex-col gap-10 px-4 sm:px-6 lg:px-8">
		<h1 class="mt-10 text-center text-3xl font-bold">Projects</h1>
		<ScrumFlow />

		<Routine />

		<Life />
	</div>
</section>
