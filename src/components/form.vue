<template>
	<div class="contacts container">
		<div class="d-flex flex-row">
			<div class="promo">
				<img src="../assets/image/Megaphone.png" alt="">
				<h3>
					Contact us
				</h3>
				<p>
					This new-found knowledge may then be used by engineers to create new tools and machines,
				</p>
			</div>
			<div class="form">
				<form action="">
					<input type="text" placeholder="Name">
					<input type="text" placeholder="Phone">
					<textarea name="" id="" cols="30" rows="10" placeholder="Message"></textarea>
					<button class="d-flex flex-row justify-content-center">BUY NOW</button>
				</form>
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
	.contacts {
		padding-top: 88px;
		padding-bottom: 122px;
	}

	.contacts {
		.promo, .form {
			width: 47%;
			margin: 10px;
		}

		.form {
			padding-top: 47px;
			padding-left: 55px;
			padding-right: 47px;
			padding-bottom: 59px;
			background: #FFFFFF;
			box-shadow: 0px 15px 50px rgba(0, 0, 0, 0.1);
			border-radius: 15px;

			input, textarea {
				background: #F7F8F9;
				border-radius: 4px;
				border: none;
				width: 100%;
				margin-bottom: 10px;
			}

			input {
				padding-left: 10px;
				height: 50px;
			}

			textarea {
				padding-left: 10px;
			}

			button {
				width: 100%;
				height: 47px;
				color: white;
				background: #F9593A;
				border: none;
				border-radius: 28.5px;
			}
		}
	}
</style>
