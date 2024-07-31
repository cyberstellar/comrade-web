<script setup>

import PhoneIcon from '@/assets/icons/PhoneIcon.vue'
</script>

<template>
  <header class="header">
    <div class="container">
      <a href="#" class="logo">
        <img src="@/assets/images/logo.svg" alt="">
      </a>
      <nav class="nav">
        <ul class="list">
          <li class="list-item">
            <a href="#" class="chevron">Services</a>
            <ul class="submenu">
              <li><a href="#">Cabinet Refacing</a></li>
              <li><a href="#">Cabinet Doors Replacement</a></li>
              <li><a href="#">Thermofoil Cabinet Door Repair</a></li>
              <li><a href="#">Decorative Wall Panels</a></li>
            </ul>
          </li>
          <li class="list-item"><a href="#">Commercial</a></li>
          <li class="list-item"><a href="#">Our Process</a></li>
          <li class="list-item"><a href="#">Gallery</a></li>
          <li class="list-item"><a href="#">Areas we serve</a></li>
          <li class="list-item"><a href="#">About us</a></li>
        </ul>
      </nav>
      <a href="tel:8900" class="phone">
        <PhoneIcon />
        <span>(800) 809-7197</span>
      </a>
      <a href="#" class="estimate button">Get a free estimate</a>
      <button class="menu"></button>
    </div>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  position: fixed;
  font-size: 18px;
  height: var(--header-height);
  width: 100%;
  background-color: var(--theme-color-header-bg);
  border-radius: 0 0 8px 8px;
  z-index: 999;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  column-gap: 24px;
}

.nav {
  height: 100%;

  .list {
    display: none;
    flex-direction: row;
    justify-content: space-between;
    height: 100%;
    gap: 15px;

    .list-item {
      position: relative;

      a {
        display: flex;
        align-items: center;
        column-gap: 8px;
        height: 100%;
      }

      &:hover {
        .submenu {
          display: flex;
        }
      }

      .submenu {
        --padding: var(--m32);
        display: none;
        flex-direction: column;
        position: absolute;
        row-gap: 16px;
        padding: var(--padding);
        left: calc(var(--padding) * -1);
        background-color: var(--theme-color-button-hover);
        border-radius: 0 0 24px 24px;
        border: var(--border);
      }
    }
  }
}

.logo {
  height: 40px;

  img {
    height: 100%;
  }
}

.phone {
  --color: var(--theme-color-brand-orange);
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 0;
  color: var(--color);
  box-shadow: inset 0 0 0 1px var(--color);
  width: 40px;
  height: 40px;
  border-radius: 100%;

  svg {
    fill: var(--color);
    transition: var(--transition);
  }

  &:hover {
    background: var(--color);
    box-shadow: none;
    svg {
      fill: var(--theme-color-text-white);
    }
  }
}

.estimate {
  display: none;
}

.menu {
  display: block;
  width: 40px;
  height: 40px;
  padding: 0;
}

@media screen and (min-width: 1024px) {
  .header {
    border-radius: 0 0 48px 48px;
  }

  .logo {
    height: 60px;
  }

  .nav .list {
    display: flex !important;
  }

  .phone {
    font-size: unset;
    border: 0;
    width: auto;
    height: auto;
    box-shadow: none;

    svg {
      display: none;
    }
  }

  .estimate {
    display: block;
  }

  .menu {
    display: none;
  }
}
</style>
