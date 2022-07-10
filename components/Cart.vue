<template lang="">
    <div>
         <div class="container">
            <p> Страница обновляется, ибо роутер на бесплатном хостинге не работал</p>
     
        <div class="cart mt-5">
             <a href="/button">
<div class="cart__box">
                        <img src="~/assets/img/start.png" alt="">
                <h5 class='mt-3'>Button</h5>
               <button class='btn btn-primary mt-2 mb-4'>Открыть</button> 
            </div>
            </a>

         
          <a href="/checkbox">
            <div class="cart__box">
                <img src="~/assets/img/verified-checkbox-symbol.png" alt="">
                <h5 class='mt-3'>Checkboxs</h5>
                <button class='btn btn-primary mt-2 mb-4'>Открыть</button>
            </div>
            </a>

<a href="/select" >
            <div class="cart__box">
                        <img src="~/assets/img/choice.png" alt="">
                <h5 class='mt-3'>Select</h5>
                <button class='btn btn-primary mt-2 mb-4'>Открыть</button> 
            </div>
            </a>

<a href="/navbar">
            <div class="cart__box">
                        <img src="~/assets/img/menu.png" alt="">
                <h5 class='mt-3'>Navbar</h5>
                <button class='btn btn-primary mt-2 mb-4'>Navbar</button> 
            </div>
            </a>
            
            <a href="/toggle">
               <div class="cart__box">
                <img src="~/assets/img/switch.png" alt="">
                <h5 class='mt-3'>Toggle Navbar</h5>
                <button class='btn btn-primary mt-2 mb-4'>Открыть</button>
            </div>
            </a>

<a href="/vibration"> 
               <div class="cart__box">
                <img src="~/assets/img/premium-icon-vibration-5879451.png" alt="">
                <h5 class='mt-3'>Vibration</h5>
            <button class='btn btn-primary mt-2 mb-4'>Открыть</button>
            </div>
            </a>
        
        </div>
        </div>
    </div>
</template>
<script>
export default {
    methods:{
        reload(){
            window.location.reload();
        }
    }
}
</script>
<style scoped>
    
.cart__box{
  width: 100%;
  display: inline-block;
  overflow: hidden;
  margin-bottom: 20px;
  border: 1px solid rgb(219, 215, 215);
  text-align: center;
  transition-duration: 0.5s;
      z-index: 0;
}
.cart__box:hover{
    transform: translate3d(-3px,-3px,0);
    z-index: 1212;
-webkit-box-shadow: 4px 14px 8px 0px rgba(56, 56, 56, 0.55);
-moz-box-shadow: 4px 14px 8px 0px rgba(56, 56, 56, 0.55);
box-shadow: 4px 14px 8px 4px rgba(56, 56, 56, 0.55);

}

img{
    width: 100%;
    max-width: 64px;
}

a{
    text-decoration: none;
    color: black;
}

.pict{
    /* width: 100px; */
}

@media (min-width: 576px) {
    .cart__box{
        width: 49%;
    }
}

@media (min-width: 992px) {
    .cart__box{
        width: 33%;
    }
} 
@media (min-width: 1200px) {
    .cart__box{
        width: 24%;
    }
} 
</style>