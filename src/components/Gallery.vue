<script>
import { Autoplay, A11y } from 'swiper/modules'

import { Swiper, SwiperSlide } from 'swiper/vue'

import 'swiper/css'
import 'swiper/css/autoplay'

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, A11y],
    }
  },
}
</script>

<template>
  <section class="gallery">
    <div class="container">
      <div class="gallery__header">
        <h2>Gallery</h2>
        <div class="gallery__desc">
          <p>Browse our gallery to see before and after photos of our previous cabinet refacing projects. Our
            transformative work speaks for itself.</p>
          <a href="#!" class="button button--outline-white">Browse The Gallery</a>
        </div>
      </div>
      <div>
        <swiper
            :modules="modules"
            :slides-per-view="1"
            :slides-per-group="1"
            :space-between="16"
            :loop="true"
            :breakpoints="{
                '720': {
                  spaceBetween: 24,
                  slidesPerView: 2,
                  slidesPerGroup: 2
                }
              }"
        >
          <swiper-slide>
            <div class="slide img--cover">
              <span class="label">Before</span>
              <img src="@/assets/images/before.webp" alt="">
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="slide img--cover">
              <span class="label">After</span>
              <img src="@/assets/images/after.webp" alt="">
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="slide img--cover">
              <span class="label">Before</span>
              <img src="@/assets/images/before.webp" alt="">
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="slide img--cover">
              <span class="label">After</span>
              <img src="@/assets/images/after.webp" alt="">
            </div>
          </swiper-slide>
        </swiper>
      </div>
      <div>
        <div class="gallery__footer">
          <a href="#!">View The Project</a>
          <div class="gallery__controls">
            <button class="button--outline-white"></button>
            <button class="button--outline-white"></button>
          </div>
        </div>
      </div>
      <div class="bg-img img--cover">
        <img src="@/assets/images/logo-bg.svg" alt="Gallery">
      </div>
    </div>
  </section>
</template>

<style scoped>
.gallery {
  position: relative;
  background: #342f28;
  margin-top: 50px;
  padding: 50px 0;
  color: var(--theme-color-text-white);
  border-radius: var(--full-corners);
}

.container {
  display: flex;
  flex-direction: column;
  row-gap: 32px;
  position: relative;
  z-index: 1;
}

.gallery__header {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  row-gap: 16px;
  flex: 1;
}

.gallery__footer {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  row-gap: 32px;

  a {
    color: #F6F3EC;
    text-decoration: underline;
  }
}

.gallery__controls {
  display: flex;
  column-gap: 14px;

  button {
    --color: var(--theme-color-text-white);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0;
    width: 72px;
    height: 72px;

    &:hover {
      --color: var(--theme-color-brand-black);
    }

    &:after {
      content: '';
      display: block;
      width: 12px;
      height: 12px;
      border: 2px solid var(--color);
      border-left: none;
      border-bottom: none;
      transform: rotate(-135deg);
    }

    &:last-child:after {
      transform: rotate(45deg);
    }
  }
}

.gallery__desc {
  display: flex;
  flex-direction: column;
  align-items: start;
  row-gap: 32px;
  max-width: 744px;
}

.slide {
  position: relative;
  overflow: hidden;
  border-radius: 24px;

  .label {
    position: absolute;
    top: 16px;
    left: 16px;
    padding: 8px 24px;
    background: var(--theme-color-text-white);
    color: var(--theme-color-brand-black);
    border-radius: 100px;
  }
}

.bg-img {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  opacity: 0.1;
}

@media screen and (min-width: 1440px) {
  .gallery {
    margin-top: 100px;
    padding: 100px 0;
  }

  .container {
    row-gap: 40px;
  }

  .gallery__header {
    flex-direction: row;
  }

  .gallery__footer {
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }

  .slide .label {
    top: 24px;
    left: 24px;
    padding: 16px 32px !important;
  }
}
</style>
