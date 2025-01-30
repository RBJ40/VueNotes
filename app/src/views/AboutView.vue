<template>
  <div>
    <NewList />
    <h2>{{ animal.name }}</h2>
    <img :src="animal.image" />
  </div>
</template>

<script setup>
import AnimalCard from '..components/AnimalCard.vue'
import NewList from '../components/NewList.vue'
defineProps({
  animal: Object,
})
</script>

<style scoped></style>
