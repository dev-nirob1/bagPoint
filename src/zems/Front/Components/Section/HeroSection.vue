<template>
  <section class="hero relative">
    <div class="container">
      <div class="content">
        <HeroTitle>Carry Smart. Look Sharp.
        </HeroTitle>
        <BaseParagraph>BagPoint school backpacks are designed for students who want style, comfort, and durability.
          Organize your books, laptop, and essentials with ease — wherever you go.</BaseParagraph>
        <div class="flex gap-1">
          <BaseButton class="bg-primary">Learn More</BaseButton>
          <BaseButton class="outline-btn">Buy Now</BaseButton>
        </div>
      </div>

      <div class="image">
        <!-- <BaseImage
          image="https://images.unsplash.com/photo-1491308056676-205b7c9a7dc1?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=873">
        </BaseImage> -->
        <!-- <BaseImage
          image="https://images.unsplash.com/photo-1491308056676-205b7c9a7dc1?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=873">
        </BaseImage> -->
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  color: var(--white-color);
  background: linear-gradient(to right, rgb(from var(--primary-color)r g b / 5%), rgb(from var(--primary-color)r g b / 5%)), url('https://images.unsplash.com/photo-1491308056676-205b7c9a7dc1?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=873') center / cover no-repeat;
}

.hero .container {
  display: flex;
  align-items: center;
  justify-content: start;
  height: 100%;
  width: 100%;
  padding-top: 12rem;
}

.hero .content {
  max-width: 50%;
}

.hero .image img {
  position: absolute;
  inset: 0;
  z-index: -1;
}

</style>
