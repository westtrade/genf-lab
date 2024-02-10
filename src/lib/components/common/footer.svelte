<script>
	import FooterFeedback from "./footer-feedback.svelte";
	import FooterTopMenu from "./footer-top-menu.svelte";
	import LogoWhite from "./logo-white.svelte";
</script>

<footer class="footer">
	<div class="footer__top">
		<div class="footer__left">
			<a href="/" class="footer__logo">
				<LogoWhite />
				<span class="footer__slogan">Swiss waste<br /> transformation</span>
			</a>
			<FooterTopMenu />
		</div>
		<div class="footer__right">
			<FooterFeedback />
		</div>
	</div>

	<div class="footer__bottom">
		<nav class="footer__menu">
			<a class="footer__bottom-link" href="/privacy-policy">Privacy Policy</a>
			<a class="footer__bottom-link" href="/terms-of-servicw">
				Terms of Service
			</a>
			<a class="footer__bottom-link" href="/cookies-settings">
				Cookies Settings
			</a>
		</nav>

		<div class="footer__copyright">
			&copy; 2023 Genf Lab. All right reserved.
		</div>
	</div>
</footer>

<style lang="pcss">
	:global(.footer) {
		@apply min-h-[484px] p-20 flex flex-col gap-16;
		@apply bg-[#000] text-[#fff];
	}

	:global(.footer__top) {
		@apply min-h-[206px] flex justify-between items-start;
	}

	:global(.footer__left) {
		@apply flex flex-col gap-8;
	}

	:global(.footer__right) {
	}

	:global(.footer__logo) {
		@apply flex gap-3 items-center;
	}

	:global(.footer__slogan) {
		@apply text-[13px];
	}

	:global(.footer__bottom) {
		@apply min-h-[54px] flex flex-row  justify-between pt-8;
		@apply border-t border-[#fff];
		@apply leading-[21px] text-[14px];
	}

	:global(.footer__menu) {
		@apply flex gap-6;
	}

	:global(.footer__bottom-link) {
		@apply font-normal underline;
	}

	:global(.footer__copyright) {
	}
</style>
