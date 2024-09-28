<script setup lang="ts">
import router from '@/router'
</script>

<template>
  <nav class="nav">
    <ul class="nav-list">
      <li><button @click="router.push('/')">Home</button></li>
      <li><button @click="router.push('events')">Events</button></li>
      <li><button @click="router.push('about')">About</button></li>
      <li><button @click="router.push('contact')">Contact</button></li>
      <li><button @click="router.push('login')">Login</button></li>
    </ul>
  </nav>
</template>
<style lang="css" scoped>
.nav {
  padding: 2rem;
  border: solid;
  .nav-list {
    list-style: none;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 0;
    margin: 0;
    button {
      font-size: larger;
      background: white;
      border: none;
    }
    button:hover {
      cursor: pointer;
    }
  }
}
</style>
