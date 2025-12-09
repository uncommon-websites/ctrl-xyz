<script>
	import Header from "$lib/components/Header.svelte";
	import Hero from "$lib/components/Hero.svelte";
	import Chains from "$lib/components/Chains.svelte";
	import Features from "$lib/components/Features.svelte";
	import SocialProof from "$lib/components/SocialProof.svelte";
	import Security from "$lib/components/Security.svelte";
	import FAQ from "$lib/components/FAQ.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<div class="min-h-screen bg-[#FAFAFA] text-black font-sans selection:bg-black selection:text-white">
	<Header />
	<main>
		<Hero />
		<Chains />
		<Features />
		<SocialProof />
		<Security />
		<FAQ />
	</main>
	<Footer />
</div>

