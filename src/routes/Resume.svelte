<script lang='ts'>
	import resume from '$lib/assets/resume.pdf';
	import { ArrowDownCircle } from '@steeze-ui/heroicons';
	import { Icon } from '@steeze-ui/svelte-icon';
</script>

<section class='flex w-full flex-col gap-10 bg-white scroll-mt-16' id='resume'>
	<h1 class='mt-10 text-center text-3xl font-bold'>Resume</h1>
	<div class='mx-auto max-w-7xl px-4 sm:px-6 lg:px-8 flex flex-col items-center gap-10'>
		<a
			class='inline-flex items-center gap-x-1.5 rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600'
			download href={resume}>
			Download
			<Icon class='h-6 w-6' src={ArrowDownCircle} />
		</a>

		<embed height='2100px' src={resume} width='800px' />
	</div>
</section>