<script lang="ts">
	import '../app.css';
	interface Props {
		children?: import('svelte').Snippet;
	}

	let { children }: Props = $props();
</script>

<html class="scroll-smooth" lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta content="width=device-width, initial-scale=1.0" name="viewport" />
		<title>Stefane Fivaz - Portfolio</title>
		<meta content="Portfolio" name="description" />
	</head>
	<body>
		{@render children?.()}
	</body>
</html>
