<template>
	<div class="getting-started">
		<div class="container">
			<div class="content d-flex flex-row justify-content-center">
				<span>Ready to get started?</span>
				<a href="#" class="round-btn d-flex justify-content-center align-items-center">READ FAQ</a>
				<a href="#" class="round-btn round-btn--red d-flex justify-content-center align-items-center">REQUEST</a>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'GetStarted',
	}
</script>

<style lang="scss">
	.getting-started {
		padding: 116px 0;
		background-image: url('../assets/image/bg2.png');
		background-size: cover;
	}

	.content {
		background: #FFFFFF;
		border-radius: 8px;
		padding: 66px 170px;

		span {
			font-size: 24px;
			line-height: 32px;
		}
	}

	.round-btn {
		margin: 0 20px;
		width: 147px;
		height: 42px;
		left: calc(50% - 147px/2 + 56.5px);
		bottom: 1671px;

		border: 2px solid #EDEDED;
		box-sizing: border-box;
		border-radius: 26px;
		font-weight: bold;
		font-size: 12px;
		color: #F05638;

		&--red {
			font-weight: bold;
			font-size: 12px;

			/* identical to box height */
			text-align: center;
			letter-spacing: 2.4px;
			background: #F05638;
			color: white;
		}
	}
</style>
