<script lang="ts">
	import profile from '$lib/assets/profile.webp';
</script>

<div
	class="liquid-avatar flex aspect-square h-auto w-80 flex-shrink-0 items-center justify-center overflow-hidden border-4 border-purple-600"
>
	<img alt="profile" src={profile} />
</div>

<style>
	.liquid-avatar {
		animation: liquid 8s ease-in-out infinite;
		transition: all 1s ease-in-out;
		border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
	}

	@keyframes liquid {
		0% {
			border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
		}

		50% {
			border-radius: 30% 60% 70% 40%/50% 60% 30% 60%;
		}

		to {
			border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
		}
	}
</style>
