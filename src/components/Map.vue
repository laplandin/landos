<template>
	<div class="map">
		<div class="description d-flex flex-column">
			<h2>Our contacts</h2>
			<p>This new-found knowledge may then be used by engineers to create new tools and machines,</p>
		</div>
		<iframe src="https://yandex.ru/map-widget/v1/?um=constructor%3Ad35c828e8e74c556384fcb213e728bda567b226424960bdc474db46733bd6869&amp;source=constructor" width="100%" height="400" frameborder="0"></iframe>
	</div>
</template>

<script>
	export default {
		name: '',
	}
</script>

<style lang="scss" scoped>
	.map {
		position: relative;

		.description {
			padding-top: 40px;
			background: linear-gradient(180deg, rgba(235, 242, 243, 0.9) 28.65%, rgba(218, 218, 218, 0) 100%);
			width: 100%;
			position: absolute;
			top: 0;
			left: 0;
			right: 0;
			bottom: 0;
		}
	}
</style>
