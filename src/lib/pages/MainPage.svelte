<script lang="ts">
	import Header from '$lib/components/organisms/Header.svelte';
	import HeroSection from '$lib/components/organisms/sections/HeroSection.svelte';
	import SubHeroMenuSection from '$lib/components/organisms/sections/SubHeroMenuSection.svelte';
	import MoreThanBotSection from '$lib/components/organisms/sections/MoreThanBotSection.svelte';
	import PromotersSection from '$lib/components/organisms/sections/PromotersSection.svelte';
	import PromoBtlSection from '$lib/components/organisms/sections/PromoBTLSection.svelte';
	import MysteryShopperSection from '$lib/components/organisms/sections/MysteryShopperSection.svelte';
	import LoyaltySection from '$lib/components/organisms/sections/LoyaltySection.svelte';
	import WhatYouGetSection from '$lib/components/organisms/sections/WhatYouGetSection.svelte';
	import AiAgent from '$lib/components/organisms/sections/AIAgent.svelte';
</script>

<Header></Header>
<main>
	<HeroSection></HeroSection>
	<SubHeroMenuSection></SubHeroMenuSection>
	<MoreThanBotSection></MoreThanBotSection>
	<PromotersSection></PromotersSection>
	<PromoBtlSection></PromoBtlSection>
	<MysteryShopperSection></MysteryShopperSection>
	<LoyaltySection></LoyaltySection>
	<WhatYouGetSection></WhatYouGetSection>
	<AiAgent></AiAgent>
</main>
