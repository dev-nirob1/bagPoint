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
  <section class="hero relative flex-center">
    <div class="overlay"></div>
    <div class="container">
      <div class="medium-2 gap-2 align-center">
        <div class="content">
          <HeroTitle>Meet BagPoint - <br>Your Everyday Backpack.</HeroTitle>
          <BaseParagraph>The perfect balance of comfort, style, and durability.
            Designed to carry everything you need, without slowing you down.</BaseParagraph>
          <div class="flex gap-1">
            <BaseButton @click="handleOpenVideoModal" class="bg-secondary">Learn More</BaseButton>
            <BaseButton @click="handleOpenFormModal" class="outline-btn">Buy Now</BaseButton>
          </div>
        </div>
        <div class="image">
          <BaseImage image="/hero.png" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  padding: 4rem 0;
  color: var(--white-color);
  background: var(--primary-color);
  z-index: 0;
}

.outline-btn {
  color: var(--white-color);
  border-color: var(--white-color);
}

.outline-btn:hover {
  border-color: var(--secondary-color);
}

.overlay {
  background: var(--white-color);
  position: absolute;
  right: 0;
  bottom: 0;
  height: 45%;
  width: 80%;
  border-top-left-radius: 100%;
  z-index: -1;
}

@media(min-width: 768px) {
  .overlay {
    width: 50%;
    height: 80%;
  }

  .hero p {
    font-size: 1.15rem;
  }
}

@media(min-width: 992px) {
  .overlay {
    width: 50%;
    height: 90%;
  }
}
</style>
