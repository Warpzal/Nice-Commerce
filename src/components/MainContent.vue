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
	</main>
</template>

<style lang="scss" scoped>
.main {
	grid-area: main1;
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
		font-size: 1.4rem;
		padding: 1rem 0;
		&:last-child {
			padding-bottom: 5rem;
		}
	}
}
</style>
