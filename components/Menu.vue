<template>
<center>
    <div class='wrapper-menu'>
    <div class='menu' ref='menu'>
            <div src="~/assets/img/text.png" alt="" @click='toggle' class='toggle'>
            +
            </div>
           <li style='--i:0'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:1'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:2'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:3'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:4'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:5'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:6'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>
           <li style='--i:7'>
             <a href="">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
              </a>
           </li>

    </div>
    </div>
    </center>
</template>
<script>
export default {
    mounted(){
        setTimeout(()=>{
              this.$refs.menu.classList.add('active')
        },1300)
    },
    methods: {
        toggle(){
    this.$refs.menu.classList.toggle('active')
        }
    },
}
</script>
<style scoped>
.wrapper-menu{
display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        max-width: 360px;
}
    .menu{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 200px;
        min-height: 200px;
        position: relative;
    }
    .toggle{
         position: absolute;
         width: 60px;
         height: 60px;
         background: black;
         z-index: 1000;
         border-radius: 50%;
         color: snow;
         font-size: 26px;
         cursor: pointer;
    }
    .menu li{
        position: absolute;
        list-style: none;
        transform-origin: 100px;
        left: 0;
        transform: rotate(0deg) translateX(100px);
        transition: 0.5s;
        transition-delay: calc(0.1s * var(--i));
    }
    .menu li a{
        display: flex;
        justify-content: center;
        align-content: center;
          transform: rotate(calc(360deg/ -8 * var(--i)));
    }
     .menu.active li{
        transform: rotate(calc(360deg/8 * var(--i)));
    }
    img{
        width: 26px;
        height: 26px;
    }
</style>