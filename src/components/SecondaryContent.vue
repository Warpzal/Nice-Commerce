<template>
	<div class="main">
		<p class="main__partners">Your Partners For</p>
		<p class="main__header main__header--2 text-fancy">
			"Oh wow, look at all the extra zeroes!" growth
		</p>
		<p class="main__paragraph">
			Sure, we're a fulfillment partner, but we like to think we're more than
			that too.
		</p>
		<p class="main__paragraph">
			We'll help you streamline your inventory, reduce returns, improve your
			conversion rates, and all that other good stuff that grows your brand,
			adds some zeroes to your bank account, and helps you sleep a little
			easier at night.
		</p>
	</div>
</template>

<style lang="scss" scoped>
.main {
	grid-area: main2;
	padding: 1rem 2rem;

	&__image-container {
		width: 100%;
		height: 20rem;
		img {
			width: 100%;
			height: 100%;
			object-fit: cover;
			object-position: center;
		}
	}
	&__partners {
		font-size: 1.6rem;
		font-weight: 600;
	}
	&__header {
		padding: 3rem 0;
	}
	&__paragraph {
		color: var(--text-color-dark);
		font-size: 1.4rem;
		padding: 1rem 0;
		&:last-child {
			padding-bottom: 5rem;
		}
	}
	@include mq(lg) {
		text-align: center;
		max-width: 80rem;
		margin: 0 auto;
		margin-top: 8rem;
	}
}
</style>
