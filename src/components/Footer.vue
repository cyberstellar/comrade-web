<script setup>

</script>

<template>
  <footer>
    <div class="container">
      <div class="column">
        <div class="cell">
          <p>Physical Address:</p>
          <a href="/">245 W. Roosevelt Rd 4 Unit 29,
            West Chicago, IL 60185</a>
        </div>
        <div class="cell">
          <p>Phone:</p>
          <a href="/">(800) 809-7197</a>
        </div>
        <div class="cell">
          <p>Hours of Operation:</p>
          <p>
            Our Online Support is available 24/7<br>
            Monday – Friday: 9:00 AM – 5:00 PM<br>
            Saturday: 9:00 AM – 2:00 PM<br>
            Sunday: Closed
          </p>
        </div>
      </div>
      <div class="column">
        <div class="cell">
          <p>Follow us:</p>
          <div class="social-icons">
            <a href="/" class="button">
              <img src="@/assets/images/yelp.svg" alt="">
            </a>
            <a href="/" class="button">
              <img src="@/assets/images/facebook.svg" alt="">
            </a>
          </div>
        </div>
        <div class="cell">
          <p>
            Brought to you by
          </p>
          <img class="sponsor" src="@/assets/images/thermoflip.webp" alt="">
        </div>
        <div class="certificates">
          <img src="@/assets/images/cert1.webp" alt="">
          <img src="@/assets/images/cert2.webp" alt="">
          <img src="@/assets/images/cert3.webp" alt="">
        </div>
        <p class="ts-xs">Copyright © 2023 Kitchen Cabinet Guys - All Rights Reserved</p>
      </div>
      <div class="column">
        <ul class="nav">
          <li><a href="/">Blog</a></li>
          <li><a href="/">Privacy Policy</a></li>
          <li><a href="/">FAQ</a></li>
          <li><a href="/">Terms & Conditions</a></li>
        </ul>
        <div class="created-by ts-xs">
          Created By <a href="/">Comrade Digital Marketing Agency</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  padding-top: 150px;
  padding-bottom: 32px;
  margin-top: -70px;
  background: #342F28;

  color: var(--theme-color-text-white);

  a {
    color: var(--theme-color-brand-orange);
  }

  .column {
    display: flex;
    flex-direction: column;
    row-gap: 24px;
    flex: 1;
  };
}

.container {
  display: flex;
}

footer .column {
  padding: 0 16px;
}

.social-icons {
  display: flex;
  column-gap: 8px;

  .button {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 48px;
    height: 48px;
    padding: 0;
  }
}

.cell {
  display: flex;
  flex-direction: column;
  row-gap: 16px;
}

.sponsor {
  height: 60px;
  width: 236px;
}

.certificates {
  display: flex;
  column-gap: 16px;
}

.nav {
  display: grid;
  grid-template-columns: 1fr 1fr;
  row-gap: 16px;

  a {
    color: var(--theme-color-text-white);
  }
}

.created-by {
  margin-top: auto;
  text-align: right;
}
</style>
