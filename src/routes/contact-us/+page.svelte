<script>
	import Footer from "$lib/components/common/footer.svelte";
	import Header from "$lib/components/common/header.svelte";
	import ContactInfoItem from "$lib/components/common/contact-info-item.svelte";
	import TopBar from "$lib/components/common/top-bar.svelte";
	import TwoColumnLayout from "$lib/components/common/two-column-layout.svelte";
	import FacebookIcon from "$lib/components/icons/facebook-icon.svelte";
	import InstagramIcon from "$lib/components/icons/instagram-icon.svelte";
	import PinterestIcon from "$lib/components/icons/pinterest-icon.svelte";
	import TiktokIcon from "$lib/components/icons/tiktok-icon.svelte";
	import Input from "$lib/components/common/forms/input.svelte";
	import Textarea from "$lib/components/common/forms/textarea.svelte";
	import Checkbox from "$lib/components/common/forms/checkbox.svelte";
</script>

<TopBar class="top-bar-light">
	<span>Use code «ECOWASTE» for 18% off 3+ items</span>
	<span>Free shipping in Switzerland</span>
	<span>15% OFF YOUR FIRST ORDER</span>
</TopBar>

<Header class="header-shadow" />

<TwoColumnLayout>
	<div slot="left" class="flex flex-col gap-16">
		<h1 class="title-1 text-black">CONTACT US</h1>

		<div class="flex flex-col gap-12">
			<div class="max-w-[304px]">
				<ContactInfoItem>
					<svelte:fragment slot="title">Adress:</svelte:fragment>
					Quai Ernest-Ansermet 14, 1205 Geneva, Switzerlan
				</ContactInfoItem>
			</div>

			<div class="flex pb-[38px]">
				<div class="max-w-[304px] grow">
					<ContactInfoItem>
						<svelte:fragment slot="title">Email:</svelte:fragment>
						info@genflab.ch
					</ContactInfoItem>
				</div>
				<div class="max-w-[304px] grow">
					<ContactInfoItem>
						<svelte:fragment slot="title">Phone number:</svelte:fragment>
						+41 (0) 78 847 77 05
					</ContactInfoItem>
				</div>
			</div>

			<div class="flex gap-7">
				<InstagramIcon />
				<PinterestIcon />
				<FacebookIcon />
				<TiktokIcon />
			</div>
		</div>
	</div>

	<div slot="right" class="flex flex-col gap-12 items-end">
		<form action="" class="max-w-[512px] w-full flex flex-col gap-6">
			<Input>
				<svelte:fragment slot="label">Name</svelte:fragment>
			</Input>
			<Input>
				<svelte:fragment slot="label">Email</svelte:fragment>
			</Input>
			<Textarea placeholder="Type your message">
				<svelte:fragment slot="label">Message</svelte:fragment>
			</Textarea>

			<Checkbox>
				<svelte:fragment slot="label">I accept the terms</svelte:fragment>
			</Checkbox>

			<div class="flex justify-center">
				<button class="button button-black"> Submit </button>
			</div>
		</form>
	</div>
</TwoColumnLayout>

<Footer />
