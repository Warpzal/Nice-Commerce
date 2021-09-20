<template>
	<section class="section">
		<p class="section__title">Much, much more than just picking and packing</p>

		<button class="section__button btn">
			<span>See everything we do</span>
			<div class="section__grid-area">
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
				<div class="section__dot"></div>
			</div>
		</button>
	</section>
</template>

<style lang="scss">
.section {
	padding: 2rem;
	text-align: center;
	&__title {
		font-size: 3rem;
		font-weight: bold;
	}
	&__button-area {
		position: relative;
	}
	&__button {
		position: relative;
		margin-top: 5rem;
		font-size: 2rem;
		padding: 1.5rem 3rem;
	}
	&__grid-area {
		position: absolute;
		width: 12rem;
		height: 12rem;
		top: -3rem;
		left: -5rem;
		z-index: -1;

		display: grid;
		gap: 0.01rem;
		grid-template-columns: repeat(10, 1fr);
		grid-template-rows: repeat(10, 1fr);
	}
	&__dot {
		width: 2px;
		height: 2px;
		background: blue;
	}
	@include mq(md) {
		padding: 5rem 2rem;
	}
	@include mq(lg) {
		padding: 10rem 2rem;
		display: flex;
		flex-direction: column;
		align-items: left;
		&__title {
			text-align: left;
			font-size: 4.8rem;
			max-width: 80%;
		}
		&__button {
			width: fit-content;
		}
	}
}
</style>
