<script lang="ts">
	import Logo from "$lib/components/common/logo.svelte";
	import HeaderCart from "./header-cart.svelte";

	let className: string = "";
	export { className as class };
</script>

<header class={`header ${className}`}>
	<a href="/" class="header__logo">
		<Logo />

		<span class="header__slogan">
			Swiss Laboratory ofeco-cosmetics in Geneva
		</span>
	</a>

	<nav class="header__menu">
		<a href="/catalog">SHOP</a>
		<a href="/about">WHO WE ARE</a>
		<a href="/partners">FOR PARTNERS</a>
		<a href="/offline">OFFLINE STORES</a>
	</nav>

	<HeaderCart />
</header>

<style lang="pcss">
	:global(.header) {
		@apply flex items-center h-20;
		@apply bg-white px-16;
	}

	:global(.header__logo) {
		@apply flex  items-center gap-4;
	}

	:global(.header__slogan) {
		@apply text-[13px] max-w-[159px] leading-[14.3px] font-normal;
	}

	:global(.header__menu) {
		@apply flex items-center gap-12 mx-auto;
		@apply font-normal text-base;
	}

	:global(.header-shadow) {
		box-shadow: 0px -1px 0px 0px #000000 inset;
	}
</style>
