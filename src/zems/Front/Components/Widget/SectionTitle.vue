<script setup>
defineProps({
  title: {
    type: String
  },
  subTitle: {
    type: String
  }
})
</script>
<template>
<div>
    <BaseTitle>{{title}}</BaseTitle>
  <BaseParagraph>{{ subTitle }}</BaseParagraph>
</div>
</template>
