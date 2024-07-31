<script setup>

</script>

<template>
  <section class="intro">
    <div class="container">
      <div class="text-group">
        <h1>Your Kitchen Refacing Solution</h1>
        <p class="ts-l">Bringing New Life to Your Kitchen Cabinets: American-Made, Family-Owned Company</p>
      </div>
      <div class="btn-group">
        <a href="/" class="button">Get Your Free Estimate</a>
        <a href="/" class="button button--outline-white">View Our Process</a>
      </div>
    </div>
    <div class="section-img">
      <img src="@/assets/images/main-bg.webp" alt="">
    </div>
    <ul></ul>
  </section>
</template>

<style scoped>
.intro {
  position: relative;
  padding-top: 238px;
  padding-bottom: 203px;
  border-radius: 0 0 72px 72px;
  color: var(--theme-color-text-white);
}

.container {
  display: flex;
  position: relative;
  flex-direction: column;
  row-gap: 40px;
  z-index: 1;
}

.text-group {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  row-gap: 16px;

  p {
    max-width: 540px;
  }
}

.btn-group {
  display: flex;
  column-gap: 16px;
  width: 490px;
  margin: 0 auto;

  .button {
    flex: 1;
  }
}

.section-img {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  filter: brightness(0.6);

  img {
    width: 100%;
    height: 100%;
    max-width: 100%;
    object-fit: cover;
  }
}
</style>
