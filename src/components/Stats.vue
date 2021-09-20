<template>
	<section class="stats">
		<p class="stats__card stats__card--1">
			<span class="stats__statistic">93%</span>
			<span class="stats__description"
				>Orders shipped in less than 12 hours</span
			>
		</p>
		<p class="stats__card stats__card--2">
			<span class="stats__statistic">100%</span>
			<span class="stats__description">Scan-based Facility</span>
		</p>
		<p class="stats__card stats__card--3">
			<span class="stats__statistic">175+</span>
			<span class="stats__description">Active Retention Automations</span>
		</p>
	</section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.stats {
	// background: blue;
	margin-top: 5rem;
	grid-area: stats;
	padding: 0 2rem;
	display: grid;
	place-items: center;
	&__card {
		padding: 1rem;
		border-radius: 1rem;
		font-size: 1.6rem;
		margin-top: 1rem;
		width: 100%;
		&--1 {
			background: #edf3fc;
		}
		&--2 {
			background: #e0f5e3;
		}
		&--3 {
			background: #ffe9e0;
		}
	}
	&__statistic {
		font-size: 3rem;
		font-weight: bold;
		padding-right: 1rem;
	}
	@include mq(sm) {
		display: flex;
		gap: 3rem;
		justify-content: center;
		&__card {
			height: 10rem;
			text-align: center;
			width: clamp(10rem, 30%, 30rem);
			* {
				display: block;
			}
		}
	}
}
</style>
