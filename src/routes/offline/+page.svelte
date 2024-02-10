<script>
	import Footer from "$lib/components/common/footer.svelte";
	import Header from "$lib/components/common/header.svelte";
	import Hero from "$lib/components/common/hero.svelte";
	import TopBar from "$lib/components/common/top-bar.svelte";
	import CartIcon from "$lib/components/icons/cart-icon.svelte";
	import SpotIcon from "$lib/components/icons/spot-icon.svelte";

	import heroBackground from "$lib/images/error-page-bg.png";
	import offlineSpotsBottomBG from "$lib/images/offline-spots-bottom.png";
</script>

<TopBar class="top-bar-light">
	<span>Use code «ECOWASTE» for 18% off 3+ items</span>
	<span>Free shipping in Switzerland</span>
	<span>15% OFF YOUR FIRST ORDER</span>
</TopBar>

<Header />
<Hero src={heroBackground}>
	<div class="offline-page__hero">
		<div class="offline-page__location">
			<SpotIcon />
			Geneva, Switzerland
		</div>

		<h1 class="title-1">
			Buy our products at partner establishments in Geneva!
		</h1>

		<div class="offline-page__hero-buttons">
			<a href="/" class="button button-white">BUY ONLINE</a>
			<a href="/contact-us" class="button button-outline">BECOME A PARTNER</a>
		</div>
	</div>
</Hero>
<main class="offline-page__main">
	<header class="offline-page__header">
		<div class="offline-page__caption">Offline stores</div>
		<h1 class="title-1">WHERE YOU CAN FIND US</h1>
	</header>
</main>

<Hero src={offlineSpotsBottomBG}>
	<div class="offline-page__hero">
		<h1 class="title-1">
			Buy our products at partner establishments in Geneva!
		</h1>

		<div class="offline-page__hero-buttons">
			<a href="/contact-us" class="button button-white">
				SHOP NOW

				<CartIcon />
			</a>
		</div>
	</div>
</Hero>
<Footer />

<style lang="pcss">
	:global(.offline-page) {
	}
	:global(.offline-page__hero) {
		@apply text-white text-center items-center;
		@apply flex flex-col gap-6;
	}

	:global(.offline-page__hero-buttons) {
		@apply flex gap-6;
	}

	:global(.offline-page__location) {
		@apply flex gap-2;
		@apply text-base font-semibold leading-6;
	}

	:global(.offline-page__main) {
		@apply h-full grow py-[112px] px-8;
	}

	:global(.offline-page__caption) {
		@apply font-semibold text-base leading-6;
	}

	:global(.offline-page__header) {
		@apply flex flex-col gap-4;
	}
</style>
