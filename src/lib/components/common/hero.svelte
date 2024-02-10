<script lang="ts">
	export let src: string;
</script>

<div class="hero">
	<div class="hero__content">
		<slot />
	</div>
	<div class="hero__background">
		<img {src} class="hero__element" />
	</div>
</div>

<style>
	:global(.hero) {
		@apply relative;
	}

	:global(.hero__content) {
		@apply absolute left-0 top-0 right-0 bottom-0 gap-6 z-10 max-w-[886px] mx-auto;
		@apply flex flex-col items-center justify-center;
	}

	:global(.hero__background) {
		@apply relative;
	}

	:global(.hero__element) {
		@apply w-full;
	}

	:global(.hero__background)::before {
		@apply absolute left-0 top-0 right-0 bottom-0;
		content: "";
		background: radial-gradient(
				46.86% 46.86% at 50% 53.14%,
				rgba(0, 0, 0, 0.5) 0%,
				rgba(0, 0, 0, 0) 100%
			),
			linear-gradient(0deg, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5));
	}
</style>
