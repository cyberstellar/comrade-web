<script setup>

</script>

<template>
  <section class="our-services">
    <div class="container">
      <h2>Our Services</h2>
      <ul class="list">
        <li class="list-item">
          <div class="list-item__img img--cover">
            <img src="@/assets/images/example1.webp" alt="Keep Your Existing Doors">
          </div>
          <div class="list-item__desc">
            <p class="subheading">Refresh Your Existing Kitchen with</p>
            <h3>Cabinet Refacing</h3>
            <p class="txt-xs">Keep Your Existing Doors</p>
            <p class="txt-s">Our cabinet refacing service transforms the appearance of your kitchen while preserving its
              original layout and the structure of your existing cabinets and drawer fronts.</p>
            <a href="#!" class="button button--outline">Learn More</a>
          </div>
        </li>
        <li class="list-item">
          <div class="list-item__img img--cover img--after">
            <img src="@/assets/images/example2.webp" alt="Keep Your Existing Doors">
          </div>
          <div class="list-item__desc">
            <p class="subheading">Replace Your Cabinet Doors with </p>
            <h3>Cabinet Door Replacement</h3>
            <p class="txt-xs">Custom-made Doors & Drawer Fronts</p>
            <p class="txt-s">If your cabinet doors and drawer fronts require a refresh, our team can manufacture new
              cabinet doors in-house. We ensure the new elements seamlessly blend with your existing kitchen, providing
              an affordable and efficient upgrade.</p>
            <a href="#!" class="button button--outline">Learn More</a>
          </div>
        </li>
        <li class="list-item">
          <div class="list-item__img img--cover">
            <img src="@/assets/images/example3.webp" alt="Keep Your Existing Doors">
          </div>
          <div class="list-item__desc">
            <p class="subheading">Renew Your Peeling Cabinet Doors with </p>
            <h3>Thermofoil Cabinet Door Repair</h3>
            <p class="txt-xs">Nationwide Shipping</p>
            <p class="txt-s">We are one of very few cabinet refacing companies who can do this service at our workshop
              here in West Chicago, without disrupting your daily routine. Just ship your peeling or delaminating doors
              and fronts and get them back updated in less time than ordering new ones. We offer 48h repairs for
              Illinois residents.</p>
            <a href="#!" class="button button--outline">Learn More</a>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.our-services {
  background: #F6F3EC;
  border-radius: var(--full-corners);
  padding-top: 50px;
  padding-bottom: 50px;
}

.container > h2 {
  text-align: center;
  margin-bottom: 32px;
}

.list {
  display: flex;
  flex-direction: column;
  row-gap: 16px;
}

.list-item {
  display: flex;
  flex-direction: column;
  background: var(--theme-color-text-white);
  padding: 16px 16px 24px;
  border-radius: 16px;
  grid-gap: 24px;

  > * {
    flex: 1;
  }
}

.list-item__desc {
  margin: 0;

  p {
    color: #5e5e5e;
  }

  .subheading {
    margin-bottom: 10px;
  }

  h3, .txt-xs {
    margin-bottom: 12px;
  }

  .txt-s {
    margin-bottom: 32px;
  }
}

.list-item__img {
  overflow: hidden;
  border-radius: 16px;
}

.img--after {
  order: 0;
}

@media screen and (min-width: 1440px) {
  .our-services {
    padding-top: 95px;
    padding-bottom: 106px;
  }

  .container > h2 {
    margin-bottom: 40px !important;
  }

  .list-item {
    flex-direction: row;
    padding: 24px;
    border-radius: 32px;
  }

  .list-item__desc {
    margin: auto 60px;

    .subheading {
      margin-bottom: 18px;
    }

    h3, .txt-xs {
      margin-bottom: 16px;
    }
  }

  .img--after {
    order: 1;
  }

  .list-item__img {
    border-radius: 16px;
  }
}
</style>
