<script lang="ts">
	let className: string = "";
	export { className as class };
</script>

<div class={`top-bar ${className}`}>
	<slot />
</div>

<style lang="pcss">
	:global(.top-bar) {
		@apply leading-9 text-[13px] flex flex-row justify-between;
		@apply px-16;
	}

	:global(.top-bar-dark) {
		@apply bg-[#121212] text-white;
	}

	:global(.top-bar-light) {
		@apply bg-[#000] bg-[#FCF4E8];
	}
</style>
