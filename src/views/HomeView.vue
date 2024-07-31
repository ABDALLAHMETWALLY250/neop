<template>
  <div class="home">
    <div class="row">
      <div class="col-lg-5 col-md-5 col-sm-12">
        <div class="title">
          <h3 class="d-flex position-relative px-3">
            <img src="@/assets/images/coffee.png" class="cofeeImg" />

            coffee &shop
          </h3>
          <span>
            Get your ordered (better) coffee delivered to you if you want.
          </span>
          <div
            class="d-flex align-items-center gap-2 justify-content-center my-3"
          >
            <button class="buttonOff">
              Get started
              <img src="@/assets/images/ArrowDownRight.png" alt="" />
            </button>
            <p class="cart">
              <img src="@/assets/images/cart.png" alt="" />
            </p>
          </div>
        </div>
      </div>
      <div class="col-lg-7 col-md-7 col-sm-12">
        <div class="carousel">
          <div class="bg-image">
            <div class="image">
              <swiper :navigation="true" :modules="modules">
                <SwiperSlide v-for="image in Images" :key="image.id"
                  ><img src="@/assets/images/Coffee Beans.png"
                /></SwiperSlide>
              </swiper>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12">
        <slide />
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12">
        <ourProducts />
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12">
        <ourShop />
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-lg-12 col-md-12 col-sm-12">
          <ImageAnimations />
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12">
        <fotter />
      </div>
    </div>
  </div>
</template>

<script>
import ImageAnimations from "../components/imageAnimations";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/pagination";
import "@/assets/styles/style.css";
import { Pagination } from "swiper/modules";
import { Navigation } from "swiper/modules";
import "swiper/css/navigation";
import slide from "@/components/slide.vue";
import ourProducts from "@/components/OurProducts.vue";
import OurShop from "@/components/OurShop.vue";
import fotter from "@/components/fotter.vue";

export default {
  data() {
    return {
      Images: [
        {
          id: 1,
          image: "Coffee Beans.png",
        },
        {
          id: 2,
          image: "Coffee Beans.png",
        },
        {
          id: 3,
          image: "Coffee Beans.png",
        },
        {
          id: 4,
          image: "Coffee Beans.png",
        },
      ],
    };
  },
  components: {
    ImageAnimations,
    Swiper,
    SwiperSlide,
    slide,
    ourProducts,
    OurShop,
    fotter,
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
    };
  },
};
</script>

<style lang="scss" scoped>
.cart {
  background: #004876;
  margin-bottom: 0;
  border-radius: 50px;
  padding: 1rem;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}
.carousel {
  width: 100%;
  background: url("@/assets/images/bg-carsouel.png") no-repeat center center;
  height: 48rem;
  background-size: cover;
  position: relative;

  .bg-image {
    // padding: 15rem;
    position: absolute;
    background: linear-gradient(90deg, #004876 0%, #1e71a6 100%);
    background-size: cover;
    background-position: center;
    border-radius: 50%;
    right: 50%;
    top: 50%;
    transform: translate(50%, -50%);

    .image {
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      object-fit: cover;
      width: 32rem;

      img {
        width: 100%;
      }
    }
  }
}
.buttonOff {
  all: unset;
  padding: 0.5rem 4rem;
  border: 1px solid #6f4336;
  border-radius: 16px;
  color: #6f4336;
  cursor: pointer;
}
</style>
