<template>
  <div class="m-3 md:m-5 lg:m-8 sticky top-3 md:top-8">
    <div>
      <picture>
          <source media="(max-width: 600px)" srcset="/img/mobile_logo.svg">
          <img class="w-full" src="/img/desktop_logo.svg" alt="">
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

</style>