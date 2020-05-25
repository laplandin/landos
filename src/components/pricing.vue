<template>
	<div class="pricing">
		<div class="container">
			<h1 class="title">
				Choose Pricing Plan
			</h1>
			<p class="description">
				This new-found knowledge may then be used by engineers to create new tools and machines,
			</p>
			<div class="price-list d-flex flex-row justify-content-center">
				<div v-for="card in price" :class="`price-card ${card.popular ? 'popular' : ''}`">
					<h5>{{card.title}}</h5>
					<div class="card-price">
						<span class="currency">$</span>
						<span class="price">{{card.price}}</span>
						<span class="period">/mo</span>
					</div>
					<p><strong>{{card.projects}}</strong> Projects</p>
					<p><strong>{{card.images}}</strong> Projects</p>
					<p><strong>{{card.support}}</strong> Projects</p>
					<a href="#" class="price-buy d-flex justify-content-center align-items-center">
						BUY NOW
					</a>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Price',
		data: function() {
		    return {
		        price: [
					{
					    title: 'BASIC PLAN',
						price: 29,
						projects: 5,
						images: 20,
						support: '9/5',
					},
                    {
                        title: 'TEAM PLAN',
                        price: 59,
                        projects: 10,
                        images: 40,
                        support: '12/7',
						popular: true,
                    },
                    {
                        title: 'CORPORATE PLAN',
                        price: 199,
                        projects: 'Unlimited',
                        images: 'Unlimited',
                        support: '24/7',
                    }
				]
			}
		}
	}
</script>

<style lang="scss" scoped>
	.pricing {
		padding: 70px 0 180px;
		background-image: url('../assets/image/bg1.png');
		background-size: cover;
	}
	.title {
		font-size: 36px;
		line-height: 48px;
	}

	.description {
		font-size: 14px;
		line-height: 26px;
		margin-bottom: 52px;
	}

	.price-card {
		padding: 69px 80px;
		width: 310px;
		height: 400px;
		background: #F8F8F8;
		border-radius: 6px;
		margin-top: 28px;

		h5 {
			text-align: center;
			letter-spacing: 2.4px;
			font-size: 12px;
			line-height: 15px;
		}

		.currency {
			font-size: 38px;
			line-height: 48px;
			vertical-align: top;
		}

		.price {
			font-size: 74px;
			line-height: 91px;
			color: #212121;
			vertical-align: center;
		}

		.period {
			color: #9FA3A7;
			font-size: 20px;
			line-height: 25px;
		}

		p {
			font-size: 13px;
			line-height: 16px;
		}

		.price-buy {
			border: 1px solid #9FA3A7;
			box-sizing: border-box;
			border-radius: 100px;
			color:  #525252;
			height: 46px;
			border-radius: 23px;
			font-size: 12px;
		}

		&.popular {
			margin-top: 0;
			width: 355px;
			height: 455px;
			background-color: white;

			.price-buy {
				background-color: #F9593A;
				color: white;
			}
		}
	}
</style>
