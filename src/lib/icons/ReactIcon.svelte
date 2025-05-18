<script lang="ts">
	interface Props {
		class?: string;
	}

	let { class: className = '' }: Props = $props();
</script>

<svg class={className} viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg">
	<rect fill="#fff" rx="15%" />
	<circle cx="256" cy="256" fill="#61dafb" r="36" />
	<path
		d="m317.47 291.43a71 183 30 1 0 -.05.09zm-122.89.09a183 71 60 1 0 -.05-.09zm61.47 35.43a183 71 0 1 0 -.1 0z"
		fill="none"
		stroke="#61dafb"
		stroke-width="18"
	/>
</svg>
