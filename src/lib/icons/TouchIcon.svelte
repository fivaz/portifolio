<script lang="ts">
	interface Props {
		class?: string;
	}

	let { class: className = '' }: Props = $props();
</script>

<svg aria-hidden="true" class={className} fill="none" viewBox="0 0 32 32"
	><defs
		><linearGradient
			gradientUnits="userSpaceOnUse"
			id=":R6rdbqnla:-gradient"
			x1="14"
			x2="7"
			y1="14.5"
			y2="17"
			><stop stop-color="#737373"></stop><stop offset="1" stop-color="#D4D4D4" stop-opacity="0"
			></stop></linearGradient
		></defs
	><circle cx="16" cy="16" fill="#A3A3A3" fill-opacity="0.2" r="16"></circle><path
		clip-rule="evenodd"
		d="M5 4a4 4 0 014-4h14a4 4 0 014 4v13h-2V4a2 2 0 00-2-2h-1.382a1 1 0 00-.894.553l-.448.894a1 1 0 01-.894.553h-6.764a1 1 0 01-.894-.553l-.448-.894A1 1 0 0010.382 2H9a2 2 0 00-2 2v24a2 2 0 002 2h4v2H9a4 4 0 01-4-4V4z"
		fill="#A3A3A3"
		fill-rule="evenodd"
	></path><path
		d="M7 22c0-4.694 3.5-8 8-8"
		stroke="url(#:R6rdbqnla:-gradient)"
		stroke-linecap="round"
		stroke-linejoin="round"
		stroke-width="2"
	></path><path
		d="M21 20l.217-5.513a1.431 1.431 0 00-2.85-.226L17.5 21.5l-1.51-1.51a2.107 2.107 0 00-2.98 0 .024.024 0 00-.005.024l3.083 9.25A4 4 0 0019.883 32H25a4 4 0 004-4v-5a3 3 0 00-3-3h-5z"
		fill="#A3A3A3"
	></path></svg
>
