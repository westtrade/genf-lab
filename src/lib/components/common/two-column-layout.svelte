<main class="two-column-layout">
	<div class="two-column-layout__left">
		<slot name="left" />
	</div>
	<div class="two-column-layout__right">
		<slot name="right" />
	</div>
</main>

<style lang="pcss">
	:global(.two-column-layout) {
		@apply py-28 px-16 flex flex-row gap-20 h-full grow;
	}

	:global(.two-column-layout__left) {
		@apply w-1/2 grow shrink;
	}
	:global(.two-column-layout__right) {
		@apply w-1/2 grow shrink;
	}
</style>
