<template>
  <div class="body-center w-100 h-100 m-0 pb-5">
    <header>
      <nav class="navbar py-3 navbar-expand-lg navbar-dark bg-transparent fixed-top" aria-label="Tenth navbar example">
        <div class="container-fluid justify-content-center">
          <a href="" class="navbar-brand text-center fs-4 fw-semibold d-flex align-items-center gap-2">
            <img src="/cdn/images/favicon.ico" alt="">
            VuePlayer</a>
        </div>
      </nav>
    </header>
    <main class="container col-11 col-lg-9">
      <RouterView />
    </main>
  </div>
</template>

<script>
import { RouterView, RouterLink } from 'vue-router';

export default {
  components: { RouterView, RouterLink }
}
</script>

<style scoped>
/*.navbar {
  background-color: var(--body-background) !important;
}
*/
main {
  margin-top: 100px;
}
</style>
