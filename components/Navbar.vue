<template>
  <div class="mixer sticky top-3 m-3 md:m-5 lg:m-8 md:top-8">

      <div class="mixer">
        <picture>
            <source media="(max-width: 600px)" srcset="/img/mobile.jpg">
            <img src="/img/desktop.jpg" alt="">
        </picture>
      </div>
      <div class="flex justify-between uppercase mt-3 font-light lg:text-lg xl:text-2xl 2xl:text-4xl">
          <div>portfolio</div>
          <div>about us</div>
      </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
    
        }
    },
    methods: {
    },
    mounted() {
    }
}
</script>

<style>
.mixer{
 mix-blend-mode: difference;
}
</style>