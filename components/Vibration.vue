<template>
    <div>
  
           <a href="https://www.livelib.ru/reader/Fantazer1337/read"> <div class='pulse-bg'>
    <img class='telephone' src="~/assets/img/telephone-call.png" alt="">
</div>
</a> 

    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
     .telephone{
        width: 100%;
        max-width: 44px;
     }
     .pulse-bg{
       width: 100%;
        max-width: 80px;
        background: green;
        border-radius: 50%;
        padding: 15px;
        position: relative; 
     }
     .pulse-bg::after,
.pulse-bg::before {
  content: '';
  position: absolute;
  border: 2px solid green;
  left: -20px;
  opacity: 0;
  right: -20px;
  top: -20px;
  bottom: -20px;
  border-radius: 50%;
  /* animation: pulse 3.5s linear infinite; */
  animation: pulse 2.5s linear infinite;
}

.pulse-bg::after {
  /* animation-delay: 2.25s; */
  animation-delay: 1.25s;
}

@keyframes pulse {
  0% {
    transform: scale(0.5);
    opacity: 0;
  }
  50% {
    opacity: 0.7;
  }
  100% {
    transform: scale(1.2);
    opacity: 0;
  }
}
</style>