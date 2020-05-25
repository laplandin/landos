<template>
  <div class="container">
    <div class="news">
      <h3 class="title">News feed</h3>
      <h2 class="subtitle">
        Watching a movie on your smartphone can be pretty great, but who has the
        arm
      </h2>
      <div class="flex-wrap d-flex flex-row align-items-center">
        <div
          v-for="(card, index) in cards"
          :class="
            `my-card d-flex flex-column align-items-center card-${index + 1} ${
              card.dark ? 'dark' : ''
            }`
          "
        >
          <div v-if="card.active" class="new">New</div>
          <div class="img-wrapper">
            <img :src="card.img" />
          </div>
          <div class="card-content d-flex flex-column">
            <h4>{{ card.title }}</h4>
            <p>{{ card.text }}</p>
			<div class="date d-flex flex-row justify-content-between">
				<div>
					<svg class="bi bi-clock" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
						<path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm8-7A8 8 0 1 1 0 8a8 8 0 0 1 16 0z"/>
						<path fill-rule="evenodd" d="M7.5 3a.5.5 0 0 1 .5.5v5.21l3.248 1.856a.5.5 0 0 1-.496.868l-3.5-2A.5.5 0 0 1 7 9V3.5a.5.5 0 0 1 .5-.5z"/>
					</svg>
					<span>1 JUNE 2015</span>
				</div>
				<div>
					<svg class="bi bi-eye-fill" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
						<path d="M10.5 8a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0z"/>
					</svg>
					<span>343</span>
				</div>
			</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Bg1 from "../../src/assets/image/01.png";
import Bg2 from "../../src/assets/image/02.png";
import Bg3 from "../../src/assets/image/03.png";
import Bg4 from "../../src/assets/image/04.png";
import Bg5 from "../../src/assets/image/05.png";

export default {
  name: "Beautiful",
  data: function() {
    return {
      cards: [
        {
            date: '1 JUNE 2015',
          desktop: "33%",
          img: Bg1,
          title: "The number of protons",
          text:
            "Apple Inc has decided to launch the much awaited Apple Watch in the "
        },
        {
          img: Bg2,
          desktop: "33%",
          title: "Sport Stadium Birdview ",
          text:
            "Apple Inc has decided to launch the much awaited Apple Watch in the "
        },
        {
          dark: true,
          img: Bg3,
          desktop: "33%",
          title: "The number of protons",
          text:
            "Startup founders often have a more casual or offbeat attitude in their dress, office space and marketing, as compared to "
        },
        {
          img: Bg4,
          desktop: "33%",
          title: "The number of protons",
          text:
            "Apple Inc has decided to launch the much awaited Apple Watch in the"
        },
        {
          img: Bg5,
          desktop: "66%",
          title: "Sport Stadium Birdview",
          text:
            "Apple Inc has decided to launch the much awaited Apple Watch in the upcoming month of April and has already received around five to six million "
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.news {
  margin-top: 112px;
	padding-bottom: 88px;
}

.title {
  font-family: Montserrat;
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 15px;
}

.subtitle {
  font-family: Arvo;
  font-style: normal;
  font-weight: normal;
  font-size: 36px;
  line-height: 48px;
}

.cards-list {
  flex-wrap: wrap;
}

.my-card.card-5 {
  flex-basis: calc(66.666% - 20px);
}

.my-card {
  box-sizing: border-box;
  flex-basis: calc(33.333% - 20px);
  border: none !important;
  overflow: hidden;
  margin: 10px;
  border-radius: 8px;
  height: 440px;

  .card-content {
	  margin-top: auto;
	  padding: 20px;
	  height: 200px;
	  background: #F7F8F9;
	  justify-content: space-between;
  }

	&.dark  .card-content  {
		height: 200px;
		background: #292929;
		color: #9FA3A7;
	}

  .img-wrapper {
    img {
      width: 100%;
    }
  }

  .new {
    position: absolute;
    top: 6px;
    right: -30px;
    width: 100px;
    background: #ffc80a;
    transform: rotate(45deg);
    font-weight: bold;
  }

  &.active {
    box-shadow: 0 15px 50px rgba(0, 0, 0, 0.1);
    border-radius: 15px;
  }

  img {
    position: relative;
    left: -18px;
  }

  &:first-of-type {
    img {
      position: relative;
      left: -40px;
    }
  }
  &:last-of-type {
    img {
      position: relative;
      left: -32px;
    }
  }

  .next {
    img {
      left: 0;
      margin-top: 28px;
      display: flex;
    }
  }

	.date {

	}
}

.card-1 .img-wrapper {
	height: 240px;
  background: #fddd37;
	img {
		height: 100%;
		width: auto;
	}
}
.card-2 .img-wrapper  {
	height: 240px;
	img {
		height: 100%;
		width: auto;
	}
}
.card-3 .img-wrapper  {
	height: 240px;
  background: #b6e0ff;
	img {
		height: 100%;
		width: auto;
	}
}
.card-4 .img-wrapper  {
	height: 240px;
  background: linear-gradient(0deg, #fdebd5, #fdebd5);
	img {
		height: 100%;
		width: auto;
	}
}
.card-5 .img-wrapper  {
	width: 100%;
	height: 240px;
  background: #ffe1d5;
	img {
		height: 100%;
		width: auto;
	}
}
</style>
