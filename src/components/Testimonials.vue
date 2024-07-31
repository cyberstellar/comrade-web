<script setup>

import StarIcon from '@/assets/icons/StarIcon.vue'
</script>

<template>
  <section class="testimonials">
    <div class="container">
      <div class="testimonials__header">
        <h2>Testimonials</h2>
        <p>Read what our satisfied clients say about their experience with Kitchen Cabinet Guys and the quality of our work.</p>
      </div>
      <ul class="testimonials__list">
        <li class="testimonials__list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="ts-m">
            THE Kitchen Cabinet Guys ARE GREAT! HIGHLY RECOMMENDED! I found them on the Web (Google Search) and filled out a "Contact" form on a Sat. I couldn't believe that Andrei called me on Sunday morn. - I told my wife "I already like these guys!".
          </p>
          <p class="ts-s author">Christopher Torre</p>
        </li>
        <li class="testimonials__list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="ts-m">
            Andre and the team @ Kitchen Cabinet Guys LLC did a stunning transformation of my family’s kitchen. Our realtor said we easily increased the value of our home by $30k for less than a third of the cost. If anyone is considering a new kitchen,
          </p>
          <p class="ts-s author">Michael Jason</p>
        </li>
        <li class="testimonials__list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="ts-m">
            THE Kitchen Cabinet Guys ARE GREAT! HIGHLY RECOMMENDED! I found them on the Web (Google Search) and filled out a "Contact" form on a Sat. I couldn't believe that Andrei called me on Sunday morn. - I told my wife "I already like these guys!".
          </p>
          <p class="ts-s author">Christopher Torre</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.testimonials {
  padding-top: 100px;
  padding-bottom: 100px;
}

.testimonials__header {
  display: flex;
  align-items: center;
  justify-content: space-between;

  p {
    max-width: 744px;
  }
}

.testimonials__list {
  display: flex;
  column-gap: 24px;
  margin-top: 40px;
}

.testimonials__list-item {
  color: #5E5E5E;
  background: #FAFAFA;
  width: 416px;
  padding: 40px 45px 50px 40px;
  border-radius: 32px;

  .rating {
    display: flex;
    column-gap: 4px;
    margin-bottom: 32px;
  }

  .author {
    margin-top: 24px;
  }
}
</style>
