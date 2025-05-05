<script>
	import Life from './Life.svelte';
	import ScrumFlow from './ScrumFlow.svelte';
	import Routine from './Routine.svelte';
</script>

<!--scroll-mt-16 makes the anchor div appear slight under the viewport so it's not covered by the fixed navbar -->
<section class="flex w-full scroll-mt-16 flex-col gap-10 bg-white" id="projects">
	<h1 class="mt-10 text-center text-3xl font-bold">Projects</h1>

	<ScrumFlow />

	<Routine />

	<Life />
</section>
