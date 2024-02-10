<div class="info-item">
	{#if $$slots.title}
		<h2 class="info-item__title">
			<slot name="title" />
		</h2>
	{/if}

	<p>
		<slot />
	</p>
</div>

<style lang="pcss">
	:global(.info-item) {
		@apply flex flex-col gap-4;
		@apply leading-6 font-normal text-base;
	}

	:global(.info-item__title) {
		@apply font-bold text-lg leading-[27px];
	}
</style>
