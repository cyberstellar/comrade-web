<script setup>
import { ref } from 'vue'

const isActive = ref(false)

function toggleSubmenu(e) {
  e.target.closest('.list__item').querySelector('.submenu').classList.toggle('submenu--active')
}

</script>

<template>
  <header class="header" :class="{ 'header--active': isActive }">
    <div class="container">
      <a href="#!" class="logo">
        <img src="@/assets/images/logo.svg" alt="">
      </a>
      <nav class="nav" :class="{ 'nav--active': isActive }">
        <ul class="list">
          <li class="list__item">
            <div class="touch-area" @click="toggleSubmenu" />
            <a href="#!" class="chevron">Services</a>
            <div class="submenu">
              <div class="back h5 chevron--before" @click="toggleSubmenu">Back</div>
              <ul class="submenu__list">
                <li><a href="#!">Cabinet Refacing</a></li>
                <li><a href="#!">Cabinet Doors Replacement</a></li>
                <li><a href="#!">Thermofoil Cabinet Door Repair</a></li>
                <li><a href="#!">Decorative Wall Panels</a></li>
              </ul>
            </div>
          </li>
          <li class="list__item"><a href="#!">Commercial</a></li>
          <li class="list__item"><a href="#!">Our Process</a></li>
          <li class="list__item"><a href="#!">Gallery</a></li>
          <li class="list__item"><a href="#!">Areas we serve</a></li>
          <li class="list__item"><a href="#!">About us</a></li>
        </ul>
        <a href="#!" class="estimate button">Get a free estimate</a>
      </nav>
      <div class="header__actions">
        <a href="tel:8900" class="phone">(800) 809-7197</a>
        <a href="#!" class="estimate button">Get a free estimate</a>
        <button class="menu-btn" :class="{ 'menu-btn--active': isActive }" @click="isActive = !isActive"></button>
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
.header {
  display: flex;
  position: fixed;
  height: var(--header-height);
  width: 100%;
  font-size: 18px;
  border-radius: 0 0 8px 8px;
  background-color: var(--theme-color-header-bg);
  z-index: 999;

  &__actions {
    display: flex;
    column-gap: 8px;
  }

  &--active {
    border-radius: 0;
  }
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  column-gap: 40px;
}

.nav {
  --nav-bg: var(--theme-color-header-bg);
  position: fixed;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: calc(100% - var(--header-height));
  width: 100%;
  top: var(--header-height);
  left: 0;
  padding: 16px;
  background-color: var(--nav-bg);
  transform: translateX(-100%);
  transition: var(--transition);

  .list {
    display: flex;
    flex-direction: column;
    row-gap: 16px;
    height: 100%;

    .submenu {
      display: flex;
      flex-direction: column;
      gap: 24px;
      position: fixed;
      height: 100%;
      width: 100%;
      padding: 16px;
      top: 0;
      left: 0;
      background: var(--nav-bg);
      z-index: 10;
      transform: translateX(-100%);
      transition: var(--transition);

      .h5 {
        font-weight: 600;
      }

      &--active {
        transform: translateX(0);
      }

      &__list {
        display: flex;
        flex-direction: column;
        gap: 16px;
      }
    }

    .list__item {
      position: relative;
      display: flex;
      align-items: center;

      a {
        display: flex;
        align-items: center;
        height: 100%;
      }

      .touch-area {
        position: absolute;
        width: 100%;
        height: 100%;
        z-index: 9;
      }
    }
  }

  &--active {
    transform: translateX(0);
  }

  .estimate {
    display: block;
    z-index: 11;
  }
}

.logo {
  height: 40px;

  img {
    height: 100%;
  }
}

.estimate {
  display: none;
}

.menu-btn, .phone {
  background-repeat: no-repeat;
  background-position: center;
}

.menu-btn {
  display: block;
  width: 40px;
  height: 40px;
  padding: 0;
  background-image: url("@/assets/icons/menu-open.svg");
}

.menu-btn--active {
  background-image: url("@/assets/icons/menu-close.svg");
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
  border-radius: 40px;
  background-image: url("@/assets/icons/phone.svg");
}

@media screen and (min-width: 1440px) {
  .header {
    border-radius: 0 0 48px 48px;

    &__actions {
      column-gap: 24px;
    }
  }

  .logo {
    height: 60px;
  }

  .nav {
    position: static;
    transform: translateX(0);
    padding: 0;
    height: 100%;

    .list {
      flex-direction: row;
      justify-content: space-between;

      &__item {
        &:hover {
          .submenu {
            display: flex;
          }
        }

        .touch-area {
          display: none;
        }
      }

      .submenu {
        --padding: var(--m32);
        display: none;
        flex-direction: column;
        position: absolute;
        height: auto;
        width: auto;
        top: var(--header-height);
        padding: var(--padding);
        left: calc(var(--padding) * -1);
        background-color: var(--theme-color-button-hover);
        border-radius: 0 0 24px 24px;
        transform: none;
        transition: none;

        .back {
          display: none;
        }
      }
    }

    .estimate {
      display: none;
    }
  }

  .phone {
    font-size: unset;
    border: 0;
    width: auto;
    height: auto;
    box-shadow: none;
    background-image: none;
  }

  .estimate {
    display: block;
  }

  .menu-btn {
    display: none;
  }
}
</style>
