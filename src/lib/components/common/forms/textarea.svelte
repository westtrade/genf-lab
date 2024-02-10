<script lang="ts">
	export let value: string = "";
	export let placeholder: string = "";
</script>

<div class="textarea">
	<label for="" class="textarea__label">
		<slot name="label" />
	</label>
	<textarea class="textarea__element" bind:value {placeholder} />
</div>

<style lang="pcss">
	:global(.textarea) {
		@apply flex flex-col gap-2;
	}

	:global(.textarea__label) {
		@apply text-base leading-6 font-normal;
	}

	:global(.textarea__element) {
		@apply border border-[#000] bg-white placeholder:text-[#505050];
		@apply font-normal text-base leading-6;
		@apply p-3 w-full min-h-[180px];
	}
</style>
