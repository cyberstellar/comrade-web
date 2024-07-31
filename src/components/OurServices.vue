<script setup>

</script>

<template>
  <section class="our-services">
    <div class="container">
      <h2>Our Services</h2>
      <ul class="services">
        <li class="services__item">
          <div class="services__item-desc" style="order: 1">
            <p class="subheading">Refresh Your Existing Kitchen with</p>
            <h3>Cabinet Refacing</h3>
            <p class="ts-xs">Keep Your Existing Doors</p>
            <p class="ts-s">Our cabinet refacing service transforms the appearance of your kitchen while preserving its original layout and the structure of your existing cabinets and drawer fronts.</p>
            <a href="/" class="button button--outline">Learn More</a>
          </div>
          <div class="services__item-img">
            <img src="@/assets/images/example1.webp" alt="Keep Your Existing Doors">
          </div>
        </li>
        <li class="services__item">
          <div class="services__item-desc" style="order: 0">
            <p class="subheading">Replace Your Cabinet Doors with </p>
            <h3>Cabinet Door Replacement</h3>
            <p class="ts-xs">Custom-made Doors & Drawer Fronts</p>
            <p class="ts-s">If your cabinet doors and drawer fronts require a refresh, our team can manufacture new cabinet doors in-house. We ensure the new elements seamlessly blend with your existing kitchen, providing an affordable and efficient upgrade.</p>
            <a href="/" class="button button--outline">Learn More</a>
          </div>
          <div class="services__item-img">
            <img src="@/assets/images/example2.webp" alt="Keep Your Existing Doors">
          </div>
        </li>
        <li class="services__item">
          <div class="services__item-desc" style="order: 1">
            <p class="subheading">Replace Your Cabinet Doors with </p>
            <h3>Cabinet Door Replacement</h3>
            <p class="ts-xs">Custom-made Doors & Drawer Fronts</p>
            <p class="ts-s">If your cabinet doors and drawer fronts require a refresh, our team can manufacture new cabinet doors in-house. We ensure the new elements seamlessly blend with your existing kitchen, providing an affordable and efficient upgrade.</p>
            <a href="/" class="button button--outline">Learn More</a>
          </div>
          <div class="services__item-img">
            <img src="@/assets/images/example3.webp" alt="Keep Your Existing Doors">
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.our-services {
  display: flex;
  flex-direction: column;
  background: #F6F3EC;
  border-radius: 72px;
  padding-top: 95px;
  padding-bottom: 106px;
  margin-top: 100px;
}

.services {
  display: flex;
  flex-direction: column;
  row-gap: 16px;
}

.services__item {
  display: flex;
  background: var(--theme-color-text-white);
  padding: 24px;
  border-radius: 32px;
  column-gap: 72px;

  > div {
    flex: 1;
  }
}

.services__item-desc {
  display: flex;
  flex-direction: column;
  align-items: start;
  padding: 30px 0;
  color: #5e5e5e;
  row-gap: 16px;

  h3 {
    color: var(--theme-color-brand-black);
  }
}

.services__item-img {
  overflow: hidden;
  border-radius: 32px;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
