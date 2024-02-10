<div class="contact-info-item">
	{#if $$slots.title}
		<h2 class="contact-info-item__title">
			<slot name="title" />
		</h2>
	{/if}

	<p>
		<slot />
	</p>
</div>

<style lang="pcss">
	:global(.contact-info-item) {
		@apply flex flex-col gap-3;
		@apply leading-6 font-normal text-base;
	}

	:global(.contact-info-item__title) {
		@apply font-bold text-2xl leading-[33.6px];
	}
</style>
