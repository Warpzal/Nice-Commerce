<template>
	<div class="container">
		<Navigation />
		<Hero />
		<Brands />
		<Stats />
		<BasicSection1 />
		<Features />
	</div>
</template>

<script>
import Navigation from '@/components/Navigation'
import Hero from '@/components/Hero.vue'
import Brands from '@/components/Brands'
import Stats from '@/components/Stats'
import BasicSection1 from '../components/BasicSection1.vue'
import Features from '@/components/Features'

export default {
	components: {
		Navigation,
		Hero,
		Brands,
		Stats,
		BasicSection1,
		Features,
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
			'brands stats';
	}
}
</style>
