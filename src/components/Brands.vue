<template>
	<section class="brands">
		<p class="brands__heading">Join these brands</p>
		<div class="brands__logos">
			<div class="brands__logo">
				<img
					:src="
						require('@/assets/images/brands/jack-rudy-cocktail-co-logo.webp')
					"
					alt="logo"
				/>
			</div>
			<div class="brands__logo">
				<img
					:src="require('@/assets/images/brands/fits-logo.png')"
					alt="logo"
				/>
			</div>
			<div class="brands__logo">
				<img
					:src="require('@/assets/images/brands/smithey-main-logo.png')"
					alt="logo"
				/>
			</div>
			<div class="brands__logo">
				<img
					:src="require('@/assets/images/brands/rigwa-life-logo.webp')"
					alt="logo"
				/>
			</div>
		</div>
	</section>
</template>

<style lang="scss">
.brands {
	grid-area: brands;
	width: 100%;
	color: var(--text-color-dark);
	&__heading {
		padding: 2rem 2rem;
		text-align: center;
		font-size: 1.9rem;
	}
	&__logos {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}
	&__logo {
		padding: 2rem 3.5rem;
		flex-basis: clamp(9rem, 50%, 18em);
		max-height: 13rem;
		img {
			width: 100%;
			height: 100%;
			object-fit: contain;
			object-position: center;
		}
		@include mq(lg) {
			flex-basis: clamp(9rem, 25%, 18em);
		}
	}
}
</style>
