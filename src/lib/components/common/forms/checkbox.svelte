<script lang="ts">
	export let value: any = "";
</script>

<label class="checkbox">
	<div class="checkbox__control">
		<input type="checkbox" class="peer checkbox__element" bind:value />

		<div class="checkbox__check-mark peer-checked:opacity-0">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="1em"
				height="1em"
				viewBox="0 0 24 24"
			>
				<path
					fill="currentColor"
					d="m9.55 17.308l-4.97-4.97l.714-.713l4.256 4.256l9.156-9.156l.713.713z"
				/>
			</svg>
		</div>
	</div>

	<slot name="label" />
</label>

<style lang="pcss">
	:global(.checkbox) {
		@apply flex flex-row gap-1 items-center cursor-pointer;
		@apply text-sm leading-[21px] font-normal;
	}

	:global(.checkbox__element) {
		@apply opacity-0;
	}

	:global(.checkbox__control) {
		@apply relative w-4 h-4 border border-black;
	}

	:global(.checkbox__check-mark) {
		@apply absolute top-0 left-0 transition;
	}
</style>
