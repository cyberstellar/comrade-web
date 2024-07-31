<script setup>

</script>

<template>
  <section class="gallery">
    <div class="container">
      <div class="gallery__header">
        <h2>Gallery</h2>
        <div class="gallery__desc">
          <p>Browse our gallery to see before and after photos of our previous cabinet refacing projects. Our
            transformative work speaks for itself.</p>
          <a href="/public" class="button button--outline-white">Browse The Gallery</a>
        </div>
      </div>
      <div class="image-gallery">
        <div class="image-gallery__slides">
          <div class="slide">
            <img src="../assets/images/before.webp" alt="">
          </div>
          <div class="slide">
            <img src="../assets/images/after.webp" alt="">
          </div>
        </div>
        <div class="image-gallery__nav">

        </div>
      </div>
      <div class="gallery__footer">
        <a href="/public">View The Project</a>
        <div class="gallery__controls">
          <button class="button--outline-white"></button>
          <button class="button--outline-white"></button>
        </div>
      </div>
    </div>
    <div class="bg-img">
      <img src="../assets/images/logo-bg.svg" alt="Gallery">
    </div>
  </section>
</template>

<style scoped>
.gallery {
  position: relative;
  background: #342f28;
  padding-top: 100px;
  padding-bottom: 100px;
  color: var(--theme-color-text-white);
  border-radius: 72px;
  margin-top: 100px;
}

.container {
  display: flex;
  flex-direction: column;
  row-gap: 40px;
  position: relative;
  z-index: 1;
}

.gallery__header {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.gallery__footer {
  display: flex;
  align-items: center;
  justify-content: space-between;

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

.image-gallery {
  overflow: hidden;
}

.image-gallery__slides {
  display: flex;
  column-gap: 24px;

  .slide {
    position: relative;
    overflow: hidden;
    border-radius: 24px;

    &:before {
      content: 'Before';
      display: block;
      position: absolute;
      top: 24px;
      left: 24px;
      padding: 16px 32px;
      background: var(--theme-color-text-white);
      color: var(--theme-color-brand-black);
      border-radius: 100px;
    }

    &:nth-child(2) {
      &:before {
        content: 'After';
      }
    }

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}

.bg-img {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  opacity: 0.1;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
