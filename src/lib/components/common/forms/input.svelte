<script lang="ts">
	export let value: string = "";
</script>

<div class="input">
	<label for="" class="input__label">
		<slot name="label" />
	</label>
	<input type="text" class="input__element" bind:value />
</div>

<style lang="pcss">
	:global(.input) {
		@apply flex flex-col gap-2;
	}

	:global(.input__label) {
		@apply text-base leading-6 font-normal;
	}

	:global(.input__element) {
		@apply border border-[#000] bg-white placeholder:text-[#505050];
		@apply font-normal text-base leading-6;
		@apply p-3 w-full;
	}
</style>
