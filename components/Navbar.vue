<template>
  <div class="mixer flex sticky top-3 m-3 md:m-5 lg:m-8 md:top-8">
   <div class="mixer wrapper max-w-1/4">
      <div class="container">
          <div class="back side"></div>
          <div class="top side"></div>
          <div class="bottom side"></div>
          <div class="front side"></div>
      </div>
  </div>
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


.wrapper {
  perspective: 600px;
  perspective-origin: center center;
  }

.container {
  width: 40em;
  height: 10em;
  transform-style: preserve-3d;
  animation: rotate 10s infinite linear;
  }
.container:before,
.container:after {
  content: "";
  display: block;
  position: absolute;
  width: 20em;
  height: 20em;
  }
  .container:before {
    transform: rotateX(90deg);  
    }
  .container:after {
    transform: rotatey(90deg);  
    }

.side {
  position: absolute;
  width: 44em;
  height: 12em;
  }

.back { 
  transform: translateZ(-5em);
  background-image: url('/img/cube.jpg');
    background-size:90%;
    background-position: center;
    background-repeat: no-repeat;
  }
.front {
  transform: translateZ(5em);
  background-image: url('/img/cube.jpg');
    background-size:90%;
    background-position: center;
    background-repeat: no-repeat;
  }
.top {
  transform: translateY(-5em) rotateX(90deg);
  background-image: url('/img/cube.jpg');
    background-size:90%;
    background-position: center;
    background-repeat: no-repeat;
  }
.bottom {
  transform: translateY(5em) rotateX(90deg);
  background-image: url('/img/cube.jpg');
    background-size:90%;
    background-position: center;
    background-repeat: no-repeat;
  }
.left {
  transform: translateX(-5em) rotateY(90deg);
  background-image: url('/img/cube.jpg');
    background-size:90%;
    background-position: center;
    background-repeat: no-repeat;
  }

.right {
  transform: translateX(5em) rotateY(90deg);
  background-image: url('/img/cube.jpg');
  }

@keyframes rotate {
  100% {
    transform: rotateX(360deg);
  }
}



HTML, BODY {
    height: 100%;
}

BODY {
  display: flex;
  justify-content: center;
  align-items: center;
}



</style>