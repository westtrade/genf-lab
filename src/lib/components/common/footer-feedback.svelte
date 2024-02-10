<form action="" class="footer-feedback">
	<div class="footer-feedback__title">
		Get 20% off and stay updated! Join now.
	</div>

	<div class="footer-feedback__controls">
		<input
			type="email"
			placeholder="Enter your email"
			class="footer-feedback__input"
		/>
		<button class="footer-feedback__button"> Subscribe </button>
	</div>

	<div class="footer-feedback__caption">
		By subscribing, you agree to our

		<a href="/privacy-policy" target="_blank">Privacy Policy</a>
	</div>
</form>

<style class="pcss">
	:global(.footer-feedback) {
		@apply flex flex-col gap-4;
	}

	:global(.footer-feedback__title) {
		@apply font-semibold text-base leading-6 h-[72px];
	}

	:global(.footer-feedback__input) {
		@apply bg-black border border-white placeholder:text-[#B9B9B9] text-white h-12 p-3;
	}

	:global(.footer-feedback__button) {
		@apply bg-black border border-white placeholder:text-[#B9B9B9] text-white h-12 py-3 px-6;
		@apply font-normal text-base;
	}

	:global(.footer-feedback__controls) {
		@apply flex flex-row gap-4;
	}

	:global(.footer-feedback__caption) {
		@apply font-normal text-xs leading-[18px];
	}
</style>
