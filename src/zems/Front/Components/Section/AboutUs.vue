<script setup>
defineProps({
  handleOpenVideoModal: {
    type: Function
  },
  handleOpenFormModal: {
    type: Function
  }
})
</script>

<template>
  <section id="about" class="about bg-light">
    <div class="container">
      <div class="medium-2 align-center gap-2">
        <div class="content">
          <HeroTitle>The Story Behind BackPoint</HeroTitle>
          <BaseParagraph>We Crafted This Backpack From The Raw Need Of Modern Travelers. Every Stitch Tells a Story Of
            Resilence, Every Pocket a Testament To Thoughtful Design</BaseParagraph>
          <div class="flex gap-1 mt-2">
            <BaseButton @click="handleOpenVideoModal" class="bg-secondary">Learn More</BaseButton>
            <BaseButton @click="handleOpenFormModal" class="outline-btn">Buy Now</BaseButton>
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

.about p {
  font-size: 1.1rem;
}

.about .image img {
  border-radius: .75rem;
}
</style>
