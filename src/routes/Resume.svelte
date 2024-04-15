<script lang="ts">
	import { PUBLIC_RESUME_DRIVE_ID } from '$env/static/public';
	import { ArrowDownCircle } from '@steeze-ui/heroicons';
	import { Icon } from '@steeze-ui/svelte-icon';
</script>

<section class="flex w-full scroll-mt-16 flex-col items-center gap-10 bg-white" id="resume">
	<h1 class="text-center text-3xl font-bold">Resume</h1>
	<div class="container mb-20 flex flex-col items-center gap-10 px-4 sm:px-6 lg:px-8">
		<a
			class="inline-flex items-center gap-x-1.5 rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
			download
			href={`https://drive.google.com/uc?export=download&id=${PUBLIC_RESUME_DRIVE_ID}`}
		>
			Download
			<Icon class="h-6 w-6" src={ArrowDownCircle} />
		</a>

		<iframe
			allow="autoplay"
			height="1000px"
			src={`https://drive.google.com/file/d/${PUBLIC_RESUME_DRIVE_ID}/preview`}
			title="resume"
			width="100%"
		/>
	</div>
</section>
