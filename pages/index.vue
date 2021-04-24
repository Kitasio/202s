<template>
  <div class="main" style="background-color: white;">
    <img style="position:fixed; margin-top:140px;" src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/881jdm7sdnril6hn3f3l.PNG" >
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
