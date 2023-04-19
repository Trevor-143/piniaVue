<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { useAuthStore } from "@/stores/auth";

const authStore = useAuthStore()

let person = ''
if (authStore.isAuthenticated == true) {
  person = 'Your good'
} else {
  person = 'Not Good'
}

</script>

<template>
  <header>
    
      <nav>
        <div>{{person}}</div>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>

  </header>

  <RouterView />
</template>

<style scoped> 

</style>
