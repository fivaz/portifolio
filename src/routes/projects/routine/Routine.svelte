<script lang="ts">
	import ChessBackground from './ChessBackground.svelte';
	import IphoneFrame from './IphoneFrame.svelte';
	import RoutineFooter from './RoutineFooter.svelte';
	import RoutineHeader from './RoutineHeader.svelte';
	import RoutineList from './RoutineList.svelte';
</script>

<div class="rounded-lg border">
	<div class="relative isolate overflow-hidden px-6 py-24 sm:py-32 lg:overflow-visible lg:px-0">
		<div class="absolute inset-0 -z-10 overflow-hidden">
			<ChessBackground />
		</div>
		<div
			class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 lg:mx-0 lg:max-w-none lg:grid-cols-2 lg:items-start lg:gap-y-10"
		>
			<RoutineHeader />

			<div
				class="-ml-12 -mt-12 p-12 lg:sticky lg:top-4 lg:col-start-2 lg:row-span-2 lg:row-start-1 lg:overflow-hidden"
			>
				<IphoneFrame />
			</div>

			<div
				class="lg:col-span-2 lg:col-start-1 lg:row-start-2 lg:mx-auto lg:grid lg:w-full lg:max-w-7xl lg:grid-cols-2 lg:gap-x-8 lg:px-8"
			>
				<div class="lg:pr-4">
					<div class="max-w-xl text-base leading-7 text-gray-700 lg:max-w-lg">
						<RoutineList />

						<RoutineFooter />
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
