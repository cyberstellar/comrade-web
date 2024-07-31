<script setup>

</script>

<template>
  <section class="contact-form">
    <div class="container">
      <div class="contact-form__img">
        <img src="@/assets/images/form-bg.webp" alt="">
      </div>
      <div class="contact-form__text">
        <div class="contact-form__header">
          <h1>Take the First Step Towards Your Kitchen Makeover</h1>
          <p>Ready to transform your kitchen? Contact us today to get started with your free estimate!</p>
        </div>
        <form class="contact-form__form" action="">
          <input type="text" placeholder="First Name">
          <input type="text" placeholder="Last Name">
          <input type="text" placeholder="Email">
          <input type="text" placeholder="Phone">
          <input class="address" type="text" placeholder="Address">
          <input class="service" type="text" placeholder="Select Service">
          <input class="message" type="text" placeholder="Message">
          <button type="submit">Get a Free Estimate</button>
        </form>
      </div>
    </div>
    <div class="contact-form__bg">
      <img src="@/assets/images/logo-bg.svg" alt="">
    </div>
  </section>
</template>

<style scoped>
.contact-form {
  padding-top: 100px;
  padding-bottom: 100px;
  border-radius: 72px;
  overflow: hidden;
  background: #F6F3EC;
  position: relative;

  form {
    display: grid;
    row-gap: 6px;
    column-gap: 8px;
    grid-template-columns: 1fr 1fr;

    .address, .message, .service, button {
      grid-column: 1 / 3;
    }

    button {
      margin-top: 16px;
    }
  }
}

.contact-form__header {
  margin-top: 16px;
  margin-bottom: 24px;
}

.container {
  display: flex;
  position: relative;
  column-gap: 48px;
  z-index: 1;
}

.contact-form__bg {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  opacity: 0.1;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}

.contact-form__img {
  max-width: 746px;
  border-radius: 24px;
  overflow: hidden;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
