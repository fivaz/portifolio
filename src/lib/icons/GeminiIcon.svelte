<script lang="ts">
	interface Props {
		class?: string;
	}

	let { class: className = '' }: Props = $props();
</script>

<svg
	class={className}
	id="Layer_1"
	viewBox="0 0 28 28"
	xmlns="http://www.w3.org/2000/svg"
	xmlns:xlink="http://www.w3.org/1999/xlink"
	><defs
		><style>
			.cls-1 {
				fill: url(#radial-gradient);
			}
		</style><radialGradient
			cx="-576.08"
			cy="491.7"
			fx="-576.08"
			fy="491.7"
			gradientTransform="translate(-21336.18 116711.38) rotate(18.68) scale(29.8 -238.74)"
			gradientUnits="userSpaceOnUse"
			id="radial-gradient"
			r="1"
			><stop offset=".07" stop-color="#9168c0" /><stop offset=".34" stop-color="#5684d1" /><stop
				offset=".67"
				stop-color="#1ba1e3"
			/></radialGradient
		></defs
	><path
		class="cls-1"
		d="M14,28c0-1.94-.37-3.76-1.12-5.46-.72-1.7-1.72-3.19-2.98-4.45-1.26-1.26-2.74-2.25-4.44-2.97-1.7-.75-3.52-1.12-5.46-1.12,1.94,0,3.76-.36,5.46-1.09,1.7-.75,3.19-1.75,4.44-3.01,1.26-1.26,2.25-2.74,2.98-4.44.75-1.7,1.12-3.52,1.12-5.46,0,1.94.36,3.76,1.09,5.46.75,1.7,1.75,3.19,3.01,4.44,1.26,1.26,2.74,2.26,4.45,3.01,1.7.72,3.52,1.09,5.46,1.09-1.94,0-3.76.37-5.46,1.12-1.7.72-3.19,1.71-4.45,2.97s-2.26,2.74-3.01,4.45c-.72,1.7-1.09,3.52-1.09,5.46Z"
	/></svg
>
