<template>

  <div>
      <div class="crop request flex justify-center align-center">
        <div class="request-anim flex align-center"><img src="/img/request.jpg" alt=""></div>
      </div>
  </div>
</template>

<script>
export default {
  methods: {
    requestAnim: function() {
      const outer = this.$gsap.timeline({repeat: -1})
      const inner = this.$gsap.timeline({repeat: -1})

      outer.to(".request", {scaleY: 0.1, duration: .5, delay: 5})
      outer.to(".request", {scaleY: 1, duration: .5})

      inner.to(".request-anim", {scaleY: 2, duration: .5, delay: 5})
      inner.to(".request-anim", {scaleY: 1, duration: .5})
    }  
  },
  mounted() {
    this.requestAnim()
  }
}
</script>

<style>

.request {
  position: fixed;
  bottom: 5%;
  right: 5%;
}

.crop{
  padding: 0;
  mix-blend-mode: difference;
  animation-iteration-count: infinite;
  animation-duration: 3s;
  /* animation-name: cropped; */
  width: 11rem;
  height: 1.8rem;
  border: 3px solid white;
  transform: scaleY(1);
  overflow: hidden;
}

.crop > * {
  padding: 0;
  transform: scaleY(calc(1/1));
}
.request-anim{
  
  text-align: center;
  padding:0;
  mix-blend-mode: difference;
  width: 10rem;
  transform-origin: center;
  overflow: hidden;
  /* background-image: url('/img/request.jpg');  */
  /* background-repeat: no-repeat;  */
  /* background-size: 100% 3rem;  */
}

@keyframes cropped {
  from {
    --scale: 0.1;
  }

  to {
    --scale: 0.9;
  }
}

</style>