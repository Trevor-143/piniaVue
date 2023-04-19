<template>
  <main>
    <h2>Home page</h2>
    <Counter />
    <TheWelcome />
  </main>
</template>

<script>
import { useCounterStore } from "@/stores/counter";
import { useAuthStore } from "@/stores/auth"
import Counter from "@/components/Counter.vue"

export default {
  name: 'counter',
  components: {
    Counter
  }
}

// const store = useCounterStore()
// const authetication = useAuthStore()

// console.log(store.count)
// console.log(authetication.isAuthenticated)

</script>
