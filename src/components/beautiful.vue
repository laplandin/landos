<template>
  <div class="container">
    <div class="beautiful">
      <h3 class="title">AWESOME FEATURE</h3>
      <h2 class="subtitle">Beautiful and Fully Isolated</h2>
      <div class="d-flex flex-row justify-content-center">
        <div
          v-for="card in cards"
          :class="
            `my-card d-flex flex-column align-items-center ${
              card.active ? 'active' : ''
            }`
          "
        >
          <div v-if="card.active" class="new">New</div>
          <div class="img-wrapper">
            <img :src="card.img" />
          </div>
          <h4>{{ card.title }}</h4>
          <p>{{ card.text }}</p>
          <div v-if="card.active" class="next">
            <img src="../assets/icons/Arrow Right.svg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Paper from "../../src/assets/image/Paper Hand.png";
import Eyedropper from "../../src/assets/image/Eyedropper.png";
import Crown from "../../src/assets/image/Crown.png";

export default {
  name: "Beautiful",
  data: function() {
    return {
      cards: [
        {
          img: Paper,
          title: "A4 PAPER",
          text:
            "Computer manufacturer Lenovo is in hot water this week after pre-installing"
        },
        {
          active: true,
          img: Eyedropper,
          title: "EYEDROPER",
          text:
            "It seems like hundreds of new iPhone apps pop up every week, but which  "
        },
        {
          img: Crown,
          title: "CROWN",
          text:
            "Watching a movie on your smartphone can be pretty great, but who has the arm"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.beautiful {
  padding-top: 112px;
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

.my-card {
	position: relative;
  border: none !important;
  /*width: 310px;*/
  width: 310px;
  overflow: hidden;
  margin: 20px;
  padding: 62px;

  .img-wrapper {
    height: 180px;
    overflow: hidden;
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
}
</style>
