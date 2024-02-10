<script>
	import Footer from "$lib/components/common/footer.svelte";
	import Header from "$lib/components/common/header.svelte";
	import Hero from "$lib/components/common/hero.svelte";
	import TopBar from "$lib/components/common/top-bar.svelte";

	import heroBackground from "$lib/images/error-page-bg.png";
</script>

<TopBar class="top-bar-light">
	<span>Use code «ECOWASTE» for 18% off 3+ items</span>
	<span>Free shipping in Switzerland</span>
	<span>15% OFF YOUR FIRST ORDER</span>
</TopBar>

<Header />

<main class="h-full grow">
	<Hero src={heroBackground}>
		<h1 class="title-1 text-white">404 Page Not Found</h1>

		<div class="flex flex-row gap-4">
			<a href="/" class="button button-white">BACK HOME</a>
			<a href="/contact-us" class="button button-outline">CONTACT US</a>
		</div>
	</Hero>
</main>

<Footer />
