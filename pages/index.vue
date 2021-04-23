<template>
  <div class="main">
    <Navbar />
    <Botbar />

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
