<template>
	<nav class="nav">
		<div class="nav__logo-area">
			<svg
				class="nav__logo"
				version="1.1"
				id="Layer_1"
				xmlns="http://www.w3.org/2000/svg"
				xmlns:xlink="http://www.w3.org/1999/xlink"
				x="0px"
				y="0px"
				viewBox="0 0 111.63 130.45"
				style="enable-background:new 0 0 111.63 130.45;"
				xml:space="preserve"
			>
				<g>
					<polygon
						class="st0"
						points="72.1,70.47 72.1,55.63 36.05,34.72 36.05,49.65 	"
					/>
					<polygon
						class="st1"
						points="72.1,47.29 72.1,32.44 36.05,11.54 36.05,26.47 	"
					/>
					<polygon
						class="st2"
						points="0,47.29 0,32.44 36.05,11.54 36.05,26.47 	"
					/>
					<polygon
						class="st1"
						points="32.43,102.23 19.58,109.66 55.59,130.45 68.44,123.03 	"
					/>
					<polygon
						class="st2"
						points="19.58,67.52 19.58,109.66 32.43,102.23 32.43,60.09 	"
					/>
					<polygon
						class="st3"
						points="0,55.63 0,55.63 12.85,63.05 36.05,49.65 36.05,34.72 	"
					/>
					<polygon
						class="st0"
						points="12.86,63.05 12.86,105.19 0,97.77 0,55.63 	"
					/>
					<polygon
						class="st1"
						points="39.54,59.97 39.54,74.82 75.59,95.72 75.59,80.79 	"
					/>
					<polygon
						class="st0"
						points="39.54,83.16 39.54,98 75.59,118.91 75.59,103.98 	"
					/>
					<polygon
						class="st3"
						points="111.63,83.16 111.63,98 75.59,118.91 75.59,103.98 	"
					/>
					<polygon
						class="st0"
						points="79.2,28.21 92.06,20.79 56.05,0 43.2,7.42 	"
					/>
					<polygon
						class="st3"
						points="92.06,62.93 92.06,20.79 79.2,28.21 79.2,70.35 	"
					/>
					<polygon
						class="st2"
						points="111.63,74.82 111.63,74.82 98.78,67.39 75.59,80.79 75.59,95.72 	"
					/>
					<polygon
						class="st1"
						points="98.78,67.39 98.78,25.25 111.63,32.67 111.63,74.82 	"
					/>
				</g>
			</svg>
			<p class="nav__company-name">Nice Commerce</p>
		</div>
		<ul class="nav__links desktop" :class="{ 'is-invisible': !isOpen }">
			<li><a class="nav__link" href="#">About</a></li>
			<li><a class="nav__link" href="#">How It Works</a></li>
			<li><a class="nav__link" href="#">Why Nice Commerce</a></li>
			<li><a class="nav__link" href="#">Shop</a></li>
			<li><button class="nav__btn btn" href="#">Lets Chat</button></li>
			<div v-show="isOpen" @click="toggleMenu" class="overlay"></div>
		</ul>
		<ul class="nav__menu mobile">
			<i
				v-if="!isOpen"
				@click="toggleMenu"
				class="nav__hamburger fas fa-bars"
			></i>
			<i v-else @click="toggleMenu" class="nav__times fas fa-times"></i>
		</ul>
	</nav>
</template>

<script>
export default {
	data() {
		return {
			isOpen: false,
		}
	},
	methods: {
		toggleMenu() {
			this.isOpen = !this.isOpen
		},
	},
}
</script>

<style lang="scss">
.is-invisible {
	display: none !important;
}

.overlay {
	position: absolute;
	top: 100%;
	width: 100vw;
	height: 100vh;
	background: rgba(0, 0, 0, 0.6);
}

.nav {
	position: relative;
	grid-area: nav;
	display: grid;
	grid-template-columns: auto auto;
	grid-template-areas:
		'logoArea hamburgerMenu'
		'links links';
	align-items: center;

	width: 100%;
	padding: 3rem;
	font-size: 1.4rem;
	text-transform: uppercase;
	font-weight: bold;

	&__logo-area {
		grid-area: logoArea;
		display: flex;
		align-items: center;
	}
	&__company-name {
		color: var(--text-color-dark);
		font-size: 2rem;
		font-weight: bolder;
		letter-spacing: 1px;
		transform: scale(1, 1.15);
	}
	&__logo {
		cursor: pointer;
		max-width: 4rem;
		max-height: 4rem;
		margin-right: 2rem;
	}

	&__hamburger,
	&__times {
		cursor: pointer;
		font-size: 2.5rem;
	}
	&__hamburger {
		transform: scaleX(1.3);
	}
	&__menu {
		// background: orange;
		display: flex;
		justify-content: flex-end;
		grid-area: hamburgerMenu;
	}

	&__links {
		position: absolute;
		top: -100%;
		background: white;
		width: 100%;
		padding: 3rem 0;
		grid-area: links;
		display: flex;
		flex-direction: column;
		align-items: center;
		margin-top: 2rem;
		gap: 3rem;
	}
	&__link {
		&:hover {
			color: var(--primary-color);
		}
	}
	&__btn {
		text-transform: uppercase;
	}
}

@include mq(lg) {
	.overlay {
		display: none;
	}
	.nav {
		grid-template-areas: 'logoArea links';
		&__links {
			position: relative;
			top: 0;
			flex-direction: row;
			justify-content: flex-end;
			margin-top: 0rem;
			gap: 5rem;
			padding: 0;
		}
	}
	.mobile {
		display: none;
	}
	.desktop {
		display: flex !important;
	}
}

.st0 {
	fill: #3a8dde;
}
.st1 {
	fill: #00ae42;
}
.st2 {
	fill: #006e43;
}
.st3 {
	fill: #0055b8;
}
</style>
