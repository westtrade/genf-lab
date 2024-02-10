<script>
	import Footer from "$lib/components/common/footer.svelte";
	import Header from "$lib/components/common/header.svelte";
	import InfoItem from "$lib/components/common/info-item.svelte";
	import TopBar from "$lib/components/common/top-bar.svelte";
	import TwoColumnLayout from "$lib/components/common/two-column-layout.svelte";
</script>

<TopBar class="top-bar-light">
	<span>Use code «ECOWASTE» for 18% off 3+ items</span>
	<span>Free shipping in Switzerland</span>
	<span>15% OFF YOUR FIRST ORDER</span>
</TopBar>

<Header class="header-shadow" />

<TwoColumnLayout>
	<div slot="left" class="flex flex-col gap-6">
		<h1 class="title-1 text-black">FAQs</h1>
		<p class="font-normal text-lg leading-[27px]">Still have a question?</p>

		<div>
			<a href="/contact-us" class="button button-outline-black"> Contact Us </a>
		</div>
	</div>

	<div slot="right" class="flex flex-col gap-12">
		<InfoItem>
			<svelte:fragment slot="title">
				To which countries can you deliver your products?
			</svelte:fragment>
			Сказать про страны, про почтовые компании, сколько стоит
		</InfoItem>

		<InfoItem>
			<svelte:fragment slot="title">
				Do you cooperate with institutions from other countries?
			</svelte:fragment>
			Not yet, but we plan to develop further, if you are interested in cooperation
			- leave a request to discuss partnership formats
		</InfoItem>

		<InfoItem>
			<svelte:fragment slot="title">
				Does the production of coffee waste differ from the usual ones?
			</svelte:fragment>
			No, and even more, it has a better effect on the skin, besides the fact that
			you save nature by buying each product. Our products are not only eco-friendly,
			but also gentle on the skin and great for exfoliation.
		</InfoItem>

		<InfoItem>
			<svelte:fragment slot="title">
				Where can I find out more about your production?
			</svelte:fragment>
			Subscribe to our social networks, where we talk about our products and the
			process of their creation: Instagram, Facebook, TikTok
		</InfoItem>
	</div>
</TwoColumnLayout>

<Footer />
