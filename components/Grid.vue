<template>
<div class="container">
    <center> <h3>Поторопитесь, выбрать нужный вам автомобиль!</h3></center>
    <div class='wrapper__box-grid'>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Седаны</p>
            </div>
        </div>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Лифтбэки</p>
            </div>
        </div>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Минивены</p>
            </div>
        </div>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Хэтчбеки</p>
            </div>
        </div>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Универсалы</p>
            </div>
        </div>
        <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Внедорожники</p>
            </div>
        </div>
        <!-- <div class="box">
            <div class="content">
                   <img src="~/assets/img/start.png" alt="">
                   <p>Минивены7</p>
            </div>
        </div> -->
    </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .wrapper__box-grid{
        display: grid;
        width: 100%;
        overflow: hidden;
        grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
        grid-template-rows: minmax(100px, auto);
        /* margin: 20px; */
        padding: 20px;
        grid-auto-flow: dense;
        grid-gap: 10px;
    }
    .wrapper__box-grid .box{
        background: rgb(197, 196, 196);
        padding: 20px;
        font-size: 16px;
        display: grid;
        place-items: center;
        text-align: center;
        transition: all 0.3s ease-in-out;
    }
    .wrapper__box-grid .box:hover{
          background: rgb(233, 132, 132);
    }
    img{
        width:100px;
    }
    .wrapper__box-grid .box:nth-child(1){
      grid-column: span 2;
      grid-row: span 1;
    } 
    .wrapper__box-grid .box:nth-child(2){
      grid-column: span 1;
      grid-row: span 2;
    } 
    .wrapper__box-grid .box:nth-child(3){
      grid-column: span 2;
      grid-row: span 2;
    } 
    .wrapper__box-grid .box:nth-child(4){
      grid-column: span 2;
      grid-row: span 2;
    }  
    .wrapper__box-grid .box:nth-child(5){
      grid-column: span 1;
      grid-row: span 1;
    } 
    .wrapper__box-grid .box:nth-child(6){
      grid-column: span 2;
      grid-row: span 1;
    } 
    .content p{
        font-weight: 600;
        font-size: 18px;
    }
    @media(max-width: 991px){
       .wrapper__box-grid{
        grid-template-columns: repeat(auto-fill, minmax(50%, 1fr));
        grid-template-rows: minmax(auto, auto);
    }  
    .wrapper__box-grid .box{
      grid-column: unset !important;
      grid-row: unset !important;
    } 
    }

</style>