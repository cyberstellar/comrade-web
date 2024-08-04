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
      <ul class="list">
        <li class="list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="txt-m">
            THE Kitchen Cabinet Guys ARE GREAT! HIGHLY RECOMMENDED! I found them on the Web (Google Search) and filled out a "Contact" form on a Sat. I couldn't believe that Andrei called me on Sunday morn. - I told my wife "I already like these guys!".
          </p>
          <p class="txt-s author">Christopher Torre</p>
        </li>
        <li class="list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="txt-m">
            Andre and the team @ Kitchen Cabinet Guys LLC did a stunning transformation of my family’s kitchen. Our realtor said we easily increased the value of our home by $30k for less than a third of the cost. If anyone is considering a new kitchen,
          </p>
          <p class="txt-s author">Michael Jason</p>
        </li>
        <li class="list-item">
          <div class="rating">
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
            <StarIcon />
          </div>
          <p class="txt-m">
            THE Kitchen Cabinet Guys ARE GREAT! HIGHLY RECOMMENDED! I found them on the Web (Google Search) and filled out a "Contact" form on a Sat. I couldn't believe that Andrei called me on Sunday morn. - I told my wife "I already like these guys!".
          </p>
          <p class="txt-s author">Christopher Torre</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.testimonials {
  padding: 50px 0;
}

.testimonials__header {
  display: flex;
  flex-direction: column;
  row-gap: 16px;
  margin-bottom: 40px;
}

.list {
  display: flex;
  column-gap: 24px;
}

.list-item {
  color: #5E5E5E;
  background: #FAFAFA;
  padding: 24px;
  border-radius: 16px;
  width: 100%;
  max-width: 460px;

  .rating {
    display: flex;
    column-gap: 4px;
    margin-bottom: 24px;
  }

  .author {
    margin-top: 24px;
  }
}

@media screen and (min-width: 1440px) {
  .testimonials {
    padding: 100px 0;
  }

  .testimonials__header {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 32px;

    p {
      max-width: 746px;
    }
  }

  .list-item {
    padding: 40px 45px 50px 40px;
    border-radius: 32px;

    .rating {
      margin-bottom: 32px;
    }
  }
}
</style>
