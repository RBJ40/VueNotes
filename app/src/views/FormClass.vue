<template>
  <div>
    <form name="login-form" @submit.prevent="login(user)">
      <label for="username">Enter username</label>
      <input type="text" v-model="user.username" />
      <label for="password">Enter password</label>
      <input type="password" v-model="user.password" />
      <button @click="increment">Click me</button>
      <button class="submit-button" type="submit">Login</button>
    </form>
  </div>
</template>

<script setup>
import { reactive } from 'vue'
const user = reactive({ username: '', password: '' })
function login(user) {
  console.log(user)
}
</script>

<style scoped></style>
