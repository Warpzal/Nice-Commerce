<template>
	<main class="main">
		<div class="main__image-container">
			<img
				:src="require('@/assets/images/main_content/nc-customizable.gif')"
				alt="image"
				class="main__image"
			/>
		</div>
		<p class="main__header text-fancy">
			Deliver awesome customer experiences at scale
		</p>
		<p class="main__paragraph">
			Worried that using a fulfillment partner will lose that personal touch
			that makes your brand special? We were too.
		</p>
		<p class="main__paragraph">
			That's why we've made sure that every parcel that lands in your
			customers' hands is packed with the same care and attention as if it was
			in your garage.
		</p>
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
	</main>
</template>

<style lang="scss">
.main {
	padding: 2rem;
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
		padding-top: 3rem;
	}
	&__header {
		padding: 3rem 0;
		&--2 {
			padding-top: 1rem;
		}
	}
	&__paragraph {
		font-size: 1.4rem;
		padding: 1rem 0;
		&:last-child {
			padding-bottom: 5rem;
		}
	}
}
</style>
