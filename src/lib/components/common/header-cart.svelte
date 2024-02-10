<script>
	import CartIcon from "$lib/components/icons/cart-icon.svelte";
	export let counter = 0;
</script>

<div class="header-cart">
	YOUR CART
	<div class="header-cart__icon">
		<CartIcon />

		<div class="header-cart__counter">
			{counter}
		</div>
	</div>
</div>

<style lang="pcss">
	:global(.header-cart) {
		@apply flex gap-3 items-center font-normal cursor-pointer;
	}

	:global(.header-cart__icon) {
		@apply h-[46px] w-[46px] bg-[#6C3507] rounded-full relative fill-white;
		@apply flex items-center justify-center;
	}

	:global(.header-cart__counter) {
		@apply h-[19px] w-[19px]  text-[13px] bg-[#FCF4E8] rounded-full  text-[#000];
		@apply absolute -top-[6px] -right-[6px];
		@apply flex items-center justify-center;
	}
</style>
