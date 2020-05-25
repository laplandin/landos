<template>
	<div>
		<div class="jumbo">
			<div class="container">
				<div class="d-flex flex-column">
					<img class="jumbo-img" src="../assets/image/Speaker.png" alt="">
					<div class="nav d-flex flex-row">
						<img class="logo" src="../assets/logo/Logo_land.png" alt="">
						<div class="nav-links justify-content-between d-flex flex-row">
							<span>Products</span>
							<span>Blog</span>
							<span>About</span>
						</div>
					</div>
					<div class="flex-column align-items-start d-flex">
						<h1 class="title text-left">Universal Music <br> Group and Brands</h1>
						<a class="jumbo-link d-flex justify-content-center align-items-center" href="#">Learn more</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Index',

	}
</script>

<style lang="scss">
	.jumbo {
		background-image: linear-gradient(0deg, #000000, #000000);
		height: 100vh;
		vertical-align: center;
		overflow: hidden;
		padding: 55px;
		position: relative;

		.jumbo-img {
			width: 65%;
			position: absolute;
			top: -10%;
			right: -15%;
		}

		.nav {
			span {
				color: white;
			}
			.logo {
				height: 39px;
				width: auto;
				margin-right: auto;
			}
			z-index: 1;
		}

		.nav-links {
			span {
				width: 111px;
				font-size: 12px;
			}
		}

		h1 {
			margin-top: 135px;
		}

		.title {
			margin-bottom: 88px;
			font-size: 60px;
			color: white;
		}

		.jumbo-link {
			background-color: #F05638;
			height: 42px;
			width:172px;
			text-transform: uppercase;
			color: white;
			border-radius: 26px;
		}
	}
</style>
