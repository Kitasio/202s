<template>
  <div class="main" style="background-color: white;">
    <Navbar />
    <Botbar />
    <img style="margin-top:1500px; margin-left: 900px;" src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/881jdm7sdnril6hn3f3l.PNG" >
    
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
