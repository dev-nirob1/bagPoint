<template>
  <section class="hero relative">
    <div class="medium-2 gap-2 align-center container">
      <div class="content">
        <HeroTitle>Carry Smart. Look Sharp.
        </HeroTitle>
        <BaseParagraph>BagPoint school backpacks are designed for students who want style, comfort, and durability.
          Organize your books, laptop, and essentials with ease — wherever you go.</BaseParagraph>
        <div class="flex gap-1">
          <BaseButton class="bg-primary">Learn More</BaseButton>
          <BaseButton class="bg-dark">Buy Now</BaseButton>
        </div>
      </div>

      <div class="image">
        <BaseImage image="/hero.jpg"></BaseImage>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  color: var(--white-color);
}

.hero::before,
.hero::after {
  content: '';
  position: absolute;
  width: 50%;
  height: 100%;
  top: 0;
  z-index: -1;
}

.hero::before {
  left: 0;
  background: var(--secondary-color);
}

.hero::after {
  right: 0;
  background: var(--white-color);
}
</style>
