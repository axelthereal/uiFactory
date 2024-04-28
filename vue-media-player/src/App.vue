<template>
  <header>
  </header>
  <main class="container col-11 col-lg-9 body-center">
    <RouterView />
  </main>
</template>

<script>
import { RouterView, RouterLink } from 'vue-router';

export default {
  components: { RouterView, RouterLink }
}
</script>

<style scoped></style>
