<script setup>
import SectionTitle from '../Widget/SectionTitle.vue';

</script>

<template>
  <section id="specification" class="specification bg-light">
    <div class="container">
      <div class="medium-2 align-center gap-2">
        <div class="image">
          <BaseImage
            image="https://images.unsplash.com/photo-1528921581519-52b9d779df2b?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=688" />
        </div>
        <div class="content">
          <SectionTitle title="Ready for Work, Travel, and Beyond"
            subTitle="Presicion-engineered materials selected for durability and performance. Designed to withstand the rigors of travel." />
          <ul class="small-2 large-3 gap-1 mt-2">
            <ListItem>
              <i class="fas fa-weight-hanging"></i>
              <div>
                <SubTitle>Weight</SubTitle>
                <p>1.2 kg — lightweight yet durable build</p>
              </div>
            </ListItem>

            <ListItem>
              <i class="fas fa-laptop"></i>
              <div>
                <SubTitle>Laptop Compartment</SubTitle>
                <p>Fits up to 16” laptop securely</p>
              </div>
            </ListItem>

            <ListItem>
              <i class="fas fa-water"></i>
              <div>
                <SubTitle>Water Resistance</SubTitle>
                <p>Premium waterproof nylon fabric</p>
              </div>
            </ListItem>

            <ListItem>
              <i class="fas fa-cubes"></i>
              <div>
                <SubTitle>Capacity</SubTitle>
                <p>28L spacious interior for daily essentials</p>
              </div>
            </ListItem>

            <ListItem>
              <i class="fas fa-lock"></i>
              <div>
                <SubTitle>Security</SubTitle>
                <p>Hidden anti-theft pocket for valuables</p>
              </div>
            </ListItem>

            <ListItem>
              <i class="fas fa-leaf"></i>
              <div>
                <SubTitle>Material</SubTitle>
                <p>Recycled eco-friendly nylon fabric</p>
              </div>
            </ListItem>
          </ul>

        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.specification {
  padding: 3.75rem 0;
}

.specification img {
  border-radius: .75rem;
}

.specification ul li {
  gap: .75rem;
  box-shadow: var(--box-shadow);
  padding: 1rem;
  border-radius: .5rem;
}

.specification li .sub-title {
  font-size: 1rem;
  margin: .5rem 0;
}

.specification li p {
  margin: .25rem 0 0 0;
  font-size: 16px;
}

.specification li i {
  font-size: 1.25rem;
  background: var(--primary-color);
  color: var(--white-color);
  height: 2.5rem;
  width: 2.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: .25rem;
}
</style>
