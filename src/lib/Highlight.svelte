<script lang="ts">
	interface Props {
		children?: import('svelte').Snippet;
	}

	let { children }: Props = $props();
</script>

<span class="font-semibold decoration-2 hover:text-purple-700">
	{@render children?.()}
</span>
