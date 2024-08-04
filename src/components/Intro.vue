<script setup>

</script>

<template>
  <section class="intro">
    <div class="container">
      <div class="text-group">
        <h1>Your Kitchen Refacing Solution</h1>
        <p class="txt-l">Bringing New Life to Your Kitchen Cabinets: American-Made, Family-Owned Company</p>
      </div>
      <div class="btn-group">
        <a href="/" class="button">Get Your Free Estimate</a>
        <a href="/" class="button button--outline-white">View Our Process</a>
      </div>
    </div>
    <div class="section-img img--cover">
      <img src="@/assets/images/main-bg.webp" alt="">
    </div>
  </section>
</template>

<style scoped>
.intro {
  position: relative;
  padding-top: 93px;
  padding-bottom: 32px;
  border-radius: var(--bottom-corners);
  color: var(--theme-color-text-white);
}

.container {
  display: flex;
  position: relative;
  flex-direction: column;
  row-gap: 32px;
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
  flex-direction: column;
  grid-gap: 16px;
  margin: 0 auto;
  width: 100%;

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
}

@media screen and (min-width: 1440px) {
  .intro {
    padding-top: 238px;
    padding-bottom: 203px;
  }

  .container {
    row-gap: 40px;
  }

  .btn-group {
    flex-direction: row;
    width: 490px;
  }
}
</style>
