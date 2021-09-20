<template>
	<div class="container">
		<Navigation />
		<Hero />
		<Brands />
		<Stats />
		<BasicSection1 />
		<Features />
		<MainContent />
		<SecondaryContent />
		<Icons />
		<Testimonials />
	</div>
</template>

<script>
import Navigation from '@/components/Navigation'
import Hero from '@/components/Hero.vue'
import Brands from '@/components/Brands'
import Stats from '@/components/Stats'
import BasicSection1 from '../components/BasicSection1.vue'
import Features from '@/components/Features'
import MainContent from '@/components/MainContent'
import SecondaryContent from '@/components/SecondaryContent'
import Icons from '@/components/Icons'
import Testimonials from '@/components/Testimonials'

export default {
	components: {
		Navigation,
		Hero,
		Brands,
		Stats,
		BasicSection1,
		Features,
		MainContent,
		SecondaryContent,
		Icons,
		Testimonials,
	},
}
</script>

<style lang="scss">
.container {
	max-width: 1440px;
	margin: 0 auto;

	@include mq(lg) {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-areas:
			'nav nav'
			'hero hero'
			'brands stats'
			'section features'
			'main1 main1'
			'main2 main2'
			'icons icons'
			'testimonials testimonials';
	}
}
</style>
