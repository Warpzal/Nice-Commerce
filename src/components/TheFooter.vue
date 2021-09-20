<template>
	<footer class="footer">
		<div class="footer__categories">
			<div class="footer__image-container">
				<img
					:src="require('@/assets/images/nice-logomark-fade.svg')"
					alt="footer"
				/>
			</div>
			<div class="footer__category">
				<p class="footer__title">
					COMPANY
				</p>
				<div class="footer__items footer__items--1">
					<p class="footer__item">Home</p>
					<p class="footer__item">About</p>
					<p class="footer__item">How It Works</p>
					<p class="footer__item">Why Nice Commerce</p>
					<p class="footer__item">Careers</p>
					<p class="footer__item">Blog</p>
				</div>
			</div>
			<div class="footer__category">
				<p class="footer__title">
					SOCIAL
				</p>
				<div class="footer__items footer__items--2">
					<p class="footer__item">Instagram</p>
					<p class="footer__item">LinkedIn</p>
					<p class="footer__item">YouTube</p>
					<p class="footer__item">Facebook</p>
				</div>
			</div>
			<div class="footer__category">
				<p class="footer__title">
					COMPANY
				</p>
				<div class="footer__items footer__items--3">
					<p class="footer__item">Help Center</p>
					<p class="footer__item">Client Login</p>
				</div>
			</div>
		</div>
	</footer>
</template>

<style lang="scss">
.footer {
	position: relative;
	grid-area: footer;
	width: 100%;

	background: var(--text-color-dark);
	color: white;
	font-size: 1.4rem;
	padding: 2rem;
	&__image-container {
		position: absolute;
		top: 20%;
		left: 60%;
	}
	* {
		padding: 0.5rem 0;
	}
	&__categories {
		width: 100%;
	}
	&__items {
		&--1 {
			border-top: 2px solid #3794ff;
		}
		&--2 {
			border-top: 2px solid #ff7445;
		}
		&--3 {
			border-top: 2px solid #46c150;
		}
	}
	@include mq(sm) {
		&__category {
			width: 25rem;
		}
	}
	@include mq(md) {
		&__categories {
			width: 100%;
			display: flex;
			justify-content: space-around;
			gap: 5rem;
		}
		&__image-container {
			position: static;
		}
	}
}
</style>
