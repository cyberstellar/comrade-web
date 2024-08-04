<script setup>

</script>

<template>
  <footer class="footer">
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
      <div class="column grid-col">
        <div class="cell">
          <p>Follow us:</p>
          <div class="social-icons">
            <a href="/" class="button">
              <img src="../assets/icons/yelp.svg" alt="">
            </a>
            <a href="/" class="button">
              <img src="../assets/icons/facebook.svg" alt="">
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
        <p class="copyright txt-xs">Copyright © 2023 Kitchen Cabinet Guys - All Rights Reserved</p>
      </div>
      <div class="column">
        <ul class="nav">
          <li><a href="/">Blog</a></li>
          <li><a href="/">Privacy Policy</a></li>
          <li><a href="/">FAQ</a></li>
          <li><a href="/">Terms & Conditions</a></li>
        </ul>
        <div class="created-by txt-xs">
          Created By <a href="/">Comrade Digital Marketing Agency</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  padding-top: 126px;
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
  flex-direction: column;
  row-gap: 24px;
}

.footer .column {
  padding: 0 16px;
}

.grid-col {
  display: grid !important;
  grid-template-columns: 1fr 1fr;
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

.certificates, .copyright {
  grid-column: 1 / 3;
}

.nav {
  display: grid;
  grid-template-columns: 1fr 1fr;
  row-gap: 16px;
  width: 100%;

  a {
    color: var(--theme-color-text-white);
  }
}

.created-by {
  margin-top: auto;
  text-align: left;
}

@media screen and (min-width: 1440px) {
  .container {
    flex-direction: row;
  }

  .footer {
    padding-top: 150px;
  }

  .created-by {
    text-align: right;
  }

  .grid-col {
    display: flex !important;
  }
}
</style>
