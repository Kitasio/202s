<template>

  <div>
      <div class="crop absolute" style="--scale: 0.5"><div class="request-anim"><img src="/img/request.jpg" alt=""></div></div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

.crop{
  
 mix-blend-mode: difference;
  animation-iteration-count: infinite;
  animation-duration: 3s;
  /* animation-name: cropped; */
  width: 10rem;
  border:5px solid white;
  transform: scaleY(var(--scale));
  overflow: hidden;
}

.crop > * {
  transform: scaleY(calc(1/var(--scale)));
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