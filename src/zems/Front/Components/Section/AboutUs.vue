<script setup>
import { ref } from 'vue'

const items = ref([
  {
    icon: 'fa-laptop-code',
    value: 1200,
    title: 'Bags Sold',
  },
  {
    icon: 'fa-user-tie',
    value: 350,
    title: 'Happy Customers',
  },
  {
    icon: 'fa-award',
    value: 5,
    title: 'Awards Won',
  }
])
</script>

<template>
  <section class="about">
    <div class="container">
      <div class="medium-2 align-center gap-2">
        <div class="content">
          <HeroTitle>The Story Behind BackPoint</HeroTitle>
          <BaseParagraph>We Crafted This Backpack From The Raw Need Of Modern Travelers. Every Stitch Tells a Story Of
            Resilence, Every Pocket a Testament To Thoughtful Design</BaseParagraph>
          <ul class="medium-2 larger-3 gap-1 stats-content">
            <ListItem v-for="(value, i) in items" :key="i">
              <i :class="`fa-solid ${value.icon} fa-2x`"></i>
              <div>
                <SubTitle>{{ value.value }}+</SubTitle>
                <BaseParagraph>{{ value.title }}</BaseParagraph>
              </div>
            </ListItem>
          </ul>
          <div class="flex gap-1 mt-2">
            <BaseButton class="bg-secondary">Learn More</BaseButton>
            <BaseButton class="outline-btn">Watch Video</BaseButton>
          </div>
        </div>
        <div class="image">
          <BaseImage
            image="https://images.unsplash.com/photo-1528921581519-52b9d779df2b?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=688" />
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.about {
  padding: 3.75rem 0;
}

.about .image img {
  border-radius: .75rem;
}

/* stats  */
.stats-content li {
  padding: 1rem;
  border-radius: .5rem;
  background-color: var(--white-color);
  box-shadow: var(--box-shadow);
}

.stats-content i {
  color: var(--secondary-color);
}
.stats-content .sub-title {
  margin: .5rem 0;
}

.stats-content p {
  margin: 0;
  padding: 0;
}
</style>
