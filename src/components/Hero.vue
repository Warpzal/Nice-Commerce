<template>
	<section class="hero">
		<h1 class="hero__heading">No more operational headaches. Nice.</h1>
		<p class="hero__paragraph">
			Use Nice Commerce to offer quicker shipping, boost your bottom lines and
			get back to focusing on the stuff that really matters.
		</p>
		<button class="hero__btn btn">Let's Chat</button>
		<div class="hero__img-container">
			<img
				:src="require('@/assets/images/hero/nice-warehouse-delivery.jpg')"
				alt=""
				class="hero__img"
			/>
		</div>
	</section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.hero {
	grid-area: hero;
	padding-top: 6vw;
	display: flex;
	flex-direction: column;
	align-items: center;
	text-align: center;
	color: var(--text-color-dark);

	&__heading {
		text-align: center;
		font-size: 4rem;
		max-width: 50rem;
	}
	&__paragraph {
		padding: 3rem;
		font-size: 1.8rem;
		line-height: 24px;
		max-width: 60rem;
	}
	&__btn {
		font-weight: 500;
		font-size: 2.4rem;
		padding: 1.5rem 3.5rem;
	}
	&__img-container {
		margin-top: 2rem;
		img {
			width: 100%;
			object-fit: contain;
			object-position: center;
		}
	}
	@include mq(lg) {
		&__heading {
			font-size: 5.2rem;
		}
		&__paragraph {
			font-size: 2rem;
		}
	}
}
</style>
