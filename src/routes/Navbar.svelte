<script lang="ts">
	import { page } from '$app/stores';
	import { slide } from 'svelte/transition';

	let isMobileMenuOpen = false;

	const mobileCurrentLink = 'border-indigo-500 text-indigo-700 bg-indigo-50';

	const currentLink = 'border-indigo-500 text-gray-900';

	const defaultLink = 'border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700';

	const mobileDefaultLink = `${defaultLink} hover:bg-gray-50`;

	$: hash = $page.url.hash;
</script>

<nav class="bg-white shadow fixed top-0 left-0 right-0 z-10">
	<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
		<div class="relative flex h-16 justify-between">
			<div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
				<!-- Mobile menu button -->
				<button
					aria-controls="mobile-menu"
					aria-expanded="false"
					class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
					on:click={() => (isMobileMenuOpen = !isMobileMenuOpen)}
					type="button"
				>
					<span class="absolute -inset-0.5"></span>
					<span class="sr-only">Open main menu</span>
					<!--
                      Icon when menu is closed.

                      Menu open: "hidden", Menu closed: "block"
                    -->
					<svg
						aria-hidden="true"
						class="{isMobileMenuOpen ? 'hidden' : 'block'} h-6 w-6"
						fill="none"
						stroke="currentColor"
						stroke-width="1.5"
						viewBox="0 0 24 24"
					>
						<path
							d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
							stroke-linecap="round"
							stroke-linejoin="round"
						/>
					</svg>
					<!--
                      Icon when menu is open.

                      Menu open: "block", Menu closed: "hidden"
                    -->
					<svg
						aria-hidden="true"
						class="{isMobileMenuOpen ? 'block' : 'hidden'} h-6 w-6"
						fill="none"
						stroke="currentColor"
						stroke-width="1.5"
						viewBox="0 0 24 24"
					>
						<path d="M6 18L18 6M6 6l12 12" stroke-linecap="round" stroke-linejoin="round" />
					</svg>
				</button>
			</div>
			<div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
				<div class="flex flex-shrink-0 items-center">
					<span class="text-2xl font-extrabold">Fivaz</span>
				</div>
			</div>
			<div
				class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0"
			>
				<div class="hidden sm:ml-6 sm:flex sm:space-x-8">
					<!-- Current: "border-indigo-500 text-gray-900", Default: "border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700" -->
					<a
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
{hash === '' || hash === '#home' ? currentLink : defaultLink}"
						href="#home"
					>
						Home
					</a>
					<a
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
{hash === '#about' ? currentLink : defaultLink}"
						href="#about"
					>
						About
					</a>
					<a
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
{hash === '#projects' ? currentLink : defaultLink}"
						href="#projects"
					>
						Projects
					</a>
					<a
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
{hash === '#contact' ? currentLink : defaultLink}"
						href="#contact"
					>
						Contact
					</a>
				</div>
			</div>
		</div>
	</div>

	<!-- Mobile menu, show/hide based on menu state. -->
	{#if isMobileMenuOpen}
		<div class="sm:hidden" id="mobile-menu" transition:slide={{ duration: 500 }}>
			<div class="space-y-1 pb-4 pt-2">
				<!-- Current: "bg-indigo-50 border-indigo-500 text-indigo-700", Default: "border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700" -->
				<a
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
{hash === '' || hash === '#home' ? mobileCurrentLink : mobileDefaultLink}"
					href="#home"
				>
					Home
				</a>
				<a
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
{hash === '#about' ? mobileCurrentLink : mobileDefaultLink}"
					href="#about"
				>
					About
				</a>
				<a
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
{hash === '#projects' ? mobileCurrentLink : mobileDefaultLink}"
					href="#projects"
				>
					Projects
				</a>
				<a
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
{hash === '#contact' ? mobileCurrentLink : mobileDefaultLink}"
					href="#contact"
				>
					Contact
				</a>
			</div>
		</div>
	{/if}
</nav>
