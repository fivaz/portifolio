<script lang="ts">
	interface Props {
		class?: string;
	}

	let { class: className = '' }: Props = $props();
</script>

<svg
	class={className}
	fill="none"
	height="80"
	viewBox="0 0 80 80"
	width="80"
	xmlns="http://www.w3.org/2000/svg"
	><rect fill="currentColor" height="80" rx="16" width="80"></rect><g
		clip-path="url(#clip0_939_3624)"
		><path
			clip-rule="evenodd"
			d="M56.5598 30.7427C56.5598 20.5679 47.3209 12.3191 35.9236 12.3191C31.9709 12.3191 28.7689 20.5679 28.7689 30.7427C28.7689 33.2879 28.9686 35.7139 29.3326 37.9205H22.3261L15.0006 63.5218H35.9268V49.1694C47.3209 49.1694 56.5566 40.9174 56.5566 30.7459L56.5598 30.7427ZM35.9236 15.6935C37.9917 15.6935 39.6668 22.4325 39.6668 30.7427C39.6668 39.0528 37.9917 45.7918 35.9236 45.7918C33.8554 45.7918 32.1803 39.0528 32.1803 30.7427C32.1803 22.4325 33.8554 15.6935 35.9236 15.6935Z"
			fill="white"
			fill-rule="evenodd"
		></path><path
			clip-rule="evenodd"
			d="M56.9625 49.1694H35.9462L44.0061 63.525H65.0192L56.9625 49.1694Z"
			fill="white"
			fill-rule="evenodd"
		></path></g
	><defs
		><clipPath id="clip0_939_3624"
			><rect fill="white" height="51.2059" transform="translate(15.0002 12.3191)" width="50.0186"
			></rect></clipPath
		></defs
	></svg
>
