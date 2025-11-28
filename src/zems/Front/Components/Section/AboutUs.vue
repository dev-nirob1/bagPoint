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
          <BaseParagraph>
            We Crafted This Backpack From The Raw Need Of Modern Travelers. Every Stitch Tells a Story Of
            Resilence, Every Pocket a Testament To Thoughtful Design
          </BaseParagraph>
          <BaseParagraph>
            Built for convenience and comfort, BackPoint adapts to your journey—whether you're navigating
            busy streets, rushing to class, or exploring new places. It's not just a bag; it's a reliable companion
            designed to support your everyday adventures.
          </BaseParagraph>
          <div class="flex gap-1 mt-2">
            <BaseButton @click="handleOpenVideoModal" class="bg-primary">Learn More</BaseButton>
            <BaseButton @click="handleOpenFormModal" class="bg-dark">Buy Now</BaseButton>
          </div>
        </div>
        <div class="medium-2 gap-1">
          <div class="image">
            <BaseImage
              image="https://images.unsplash.com/photo-1521411086197-4f459beee413?q=80&w=435&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" />
          </div>
          <div class="image">
            <BaseImage
              image="https://images.unsplash.com/photo-1597800811995-7c5c236a1ba6?q=80&w=387&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" />
          </div>
          <div class="image">
            <BaseImage
              image="https://images.unsplash.com/photo-1754124183074-694e8e096476?q=80&w=1032&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" />
          </div>
          <div class="image">
            <BaseImage
              image="https://images.unsplash.com/photo-1624292981551-e3aa15c0056d?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTA3fHxiYWNrcGFjayUyMHBhZGRlZCUyMHN0cmFwc3xlbnwwfHwwfHx8MA%3D%3D" />
          </div>
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

.image {
  max-height: 280px;
  height: 100%;
}

.about .image img {
  border-radius: .75rem;
}

.about .btn.bg-primary:hover {
  background: var(--secondary-color);
  color: var(--dark-color);
}

.about .btn.bg-dark:hover {
  background: var(--primary-color);
  color: var(--white-color);
}
</style>
