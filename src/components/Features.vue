<template>
	<section class="features">
		<div class="features__box features__box--1">
			<h5 class="features__title">Same Day</h5>
			<p class="features__description">
				All standard orders placed by 2pm EST ship the same day
			</p>
		</div>
		<div class="features__box features__box--2">
			<h5 class="features__title">Unique</h5>
			<p class="features__description">
				Unique unboxing experiences for different customers
			</p>
		</div>
		<div class="features__box features__box--3">
			<h5 class="features__title">Manage</h5>
			<p class="features__description">
				Returns and inventory management
			</p>
		</div>
		<div class="features__box features__box--4">
			<h5 class="features__title">24/7</h5>
			<p class="features__description">
				24/7 access to analytics & inventory management
			</p>
		</div>
		<div class="features__box features__box--5">
			<h5 class="features__title">Multi Channel</h5>
			<p class="features__description">
				Omnichannel fulfillment & direct integration with all major cart
				platforms
			</p>
		</div>
		<div class="features__box features__box--6">
			<h5 class="features__title">Anywhere</h5>
			<p class="features__description">
				Ship to anywhere in the world with competitive rates
			</p>
		</div>
	</section>
</template>

<style lang="scss">
.features {
	padding: 5rem 2rem;
	display: grid;
	grid-template-columns: 1fr 1fr;
	gap: 3rem;
	&__box {
		width: 100%;
		height: 10rem;
		border-top: 2px solid;
		padding-bottom: 3rem;
		&--1 {
			border-color: #2066d2;
		}
		&--2 {
			border-color: #ff7445;
		}
		&--3 {
			border-color: #46c150;
		}
		&--4 {
			border-color: #3794ff;
		}
		&--5 {
			border-color: #057c66;
		}
		&--6 {
			border-color: #2066d2;
		}
	}
	&__title {
		padding: 2rem 0;
		text-transform: uppercase;
		font-weight: bold;
		color: var(--text-color-dark);
		font-size: 1.6rem;
	}
	&__description {
		font-size: 1.4rem;
	}
	@include mq(md) {
		padding: 5rem 2rem;
		grid-template-columns: repeat(3, 1fr);
	}
	@include mq(lg) {
		padding: 10rem 2rem;
	}
}
</style>
