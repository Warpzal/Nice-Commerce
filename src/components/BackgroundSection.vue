<template>
	<div class="background">
		<img :src="require('@/assets/images/hero/nice-delivery.jpg')" alt="bg" />
	</div>
</template>

<style lang="scss" scoped>
.background {
	grid-area: bg;
	margin-top: 20rem;
	img {
		width: 100%;
		height: 100%;
		object-fit: contain;
		object-position: bottom;
	}
}
</style>
