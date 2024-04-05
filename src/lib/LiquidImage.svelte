<script lang="ts">
	import profile from '$lib/assets/profile.jpeg';
</script>

<div class="liquid-avatar border-4 border-purple-600 w-full h-full overflow-hidden">
	<img
		alt="profile"
		class="relative top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2"
		src={profile}
	/>
</div>

<style>
	.liquid-avatar {
		animation: morph 8s ease-in-out infinite;
		transition: all 1s ease-in-out;
		border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
	}

	@keyframes morph {
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
