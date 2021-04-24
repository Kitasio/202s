<template>
  <div class="main" style="background-color: white;">
    <Navbar />
    <Botbar />

    <img class="w-full mx-auto mt-64" src="/img/Package.jpg" alt="">
    <img class="mb-64 w-full mx-auto mt-64" src="/img/banner.jpg" alt="">
  </div>

</template>

<script>
import Navbar from '../components/Navbar.vue'
import Botbar from '../components/Botbar.vue'
export default {
  components: {
    Navbar,
    Botbar,
  }
}
</script>

<style>
.main {
  height: 2000px;
}
</style>
