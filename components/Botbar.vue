<template>
  <div>
      <div class="crop absolute" style="--scale: 0.5"><div class="request-anim"></div></div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

.crop{
  animation-iteration-count: infinite;
  animation-duration: 3s;
  animation-name: cropped;
  width: 15rem;
  border:1px solid rgb(255, 0, 0);
  transform: scaleY(var(--scale));
  overflow: hidden;
}

.crop > * {
  transform: scaleY(calc(1/var(--scale)));
}
.request-anim{

  width: 15rem;
  height: 3rem; 
  transform-origin: center;
  overflow: hidden;
  background-image: url('/img/request.jpg'); 
  background-repeat: no-repeat; 
  background-size: 100% 3rem; 
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