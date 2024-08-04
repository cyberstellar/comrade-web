<script setup>

</script>

<template>
  <section class="contact-form">
    <div class="container">
      <div class="contact-form__img img--cover">
        <img src="@/assets/images/form-bg.webp" alt="">
      </div>
      <div class="contact-form__text">
        <div class="contact-form__header">
          <h1>Take the First Step Towards Your Kitchen Makeover</h1>
          <p>Ready to transform your kitchen? Contact us today to get started with your free estimate!</p>
        </div>
        <form class="contact-form__form" action="">
          <input class="first-name" type="text" placeholder="First Name">
          <input class="last-name" type="text" placeholder="Last Name">
          <input class="email" type="text" placeholder="Email">
          <input class="phone" type="text" placeholder="Phone">
          <input class="address" type="text" placeholder="Address">
          <select class="service" name="service" id="service">
            <option value="" selected disabled>Select Service</option>
            <option>option 1</option>
            <option>option 2</option>
            <option>option 3</option>
          </select>
          <textarea class="message" placeholder="Message"></textarea>
          <button type="submit">Get a Free Estimate</button>
        </form>
      </div>
    </div>
    <div class="bg-img img--cover">
      <img src="@/assets/images/logo-bg.svg" alt="">
    </div>
  </section>
</template>

<style scoped>
.contact-form {
  padding: 50px 0;
  border-radius: var(--full-corners);
  overflow: hidden;
  background: #F6F3EC;
  position: relative;

  form {
    display: grid;
    row-gap: 6px;
    column-gap: 8px;
    grid-template-columns: 1fr 1fr;

    > * {
      grid-column: 1 / -1;
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
  flex-direction: column;
  position: relative;
  column-gap: 48px;
  z-index: 1;
}

.contact-form__img {
  display: none;
}

.bg-img {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  opacity: 0.1;
}

.service {
  color: #757575;
}

.message {
  height: 122px;
  resize: none;
}

@media screen and (min-width: 1440px) {
  .contact-form {
    padding: 50px 0;
  }

  .container {
    flex-direction: row;
  }

  .contact-form__img {
    display: block;
    max-width: 746px;
    border-radius: 24px;
    overflow: hidden;
  }

  .contact-form__form {
    .first-name, .email {
      grid-column: 1 / 2 !important;
    }

    .last-name, .phone {
      grid-column: 2 / 3 !important;
    }
  }
}
</style>
