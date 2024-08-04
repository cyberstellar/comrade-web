<script setup>
import FinancingIcon from '@/assets/icons/FinancingIcon.vue'
import MoneyIcon from '@/assets/icons/MoneyIcon.vue'
import ClockIcon from '@/assets/icons/ClockIcon.vue'
</script>

<template>
  <section class="benefits">
    <div class="container">
      <ul class="list">
        <li class="list-item">
          <div class="list-item__icon">
            <MoneyIcon />
          </div>
          <p><b>Unlock 50% savings:</b> reface instead of replace</p>
        </li>
        <li class="list-item">
          <div class="list-item__icon">
            <ClockIcon />
          </div>
          <p>Transform your kitchen <b>in 3-5 days</b></p>
        </li>
        <li class="list-item">
          <div class="list-item__icon">
            <FinancingIcon />
          </div>
          <p>Kitchen <b>financing</b> options available</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.benefits {
  padding-top: 32px;
  padding-bottom: 32px;
}

.list {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}

.list-item {
  display: flex;
  align-items: center;
  column-gap: 16px;
  max-width: 256px;
}

.list-item__icon {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
  width: 50px;
  flex-shrink: 0;
  border-radius: 50px;
  background-color: #F6F3EC;
}

@media screen and (min-width: 1440px) {
  .list {
    flex-direction: row;
    justify-content: space-between;
  }
}
</style>
