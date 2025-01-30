<template>
  <div>
    <AnimalCard v-for="animal in animals" :key="animal.name" />
  </div>
</template>

<script setup>
const animals = [{}]
</script>

<style lang="scss" scoped></style>
