<template>
	<div class="footer">
		<div class="container">
			<div class="d-flex top-footer flex-row justify-content-between">
				<img src="../assets/logo/Logo_land.png" alt="">
				<div class="links d-flex">
					<span>products</span>
					<span>about</span>
					<span>blog</span>
					<span>contact</span>
				</div>
				<div class="socials d-flex flex-row align-items-center">
					<img src="../assets/icons/Shape-1.svg" alt="">
					<img src="../assets/icons/Shape.svg" alt="">
					<img src="../assets/icons/f_1_.svg" alt="">
					<img src="../assets/icons/Mask.svg" alt="">
				</div>
			</div>
			<div class="line">

			</div>
			<div class="copyright d-flex justify-content-center">
				© 2019 Landing. All rights reserved.
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: '',
	}
</script>

<style lang="scss" scoped>
	.footer {
		background: #000000;
	}

	.top-footer {
		padding: 72px 0;
	}

	.links {
		color: white;

		span {
			margin: 30px;
		}
	}
	.socials {
		img {
			margin: 10px;
		}
	}

	.line {
		border: 1px solid #4F4F4F;
		height: 1px;
	}

	.copyright {
		padding: 62px;
		color: rgba(200, 200, 200, 0.5);
	}
</style>
