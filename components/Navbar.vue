<template lang="">
    <div>
         
            <div class="header__nav_row">   
         <a href="" class="header__logo">
            <img src="~/assets/img/php.png" alt="">
         </a>
         <div class='header__burger'>
            <img @click='toggleMenu' class="header__burger-img" src="~/assets/img/menu.png" alt="">
         </div>
         <div class="header__nav active">
         <ul>
            <li><a href="#">checkbox.html</a></li>
            <li><a href="#">checkbox2.html</a></li>
            <li><a href="#">radio.html</a></li>
            <li><a href="#">select.html</a></li>
         </ul>

         <div class="header__nav__btn">
            <a href="">
            <button class="header__nav__btn_green">Sign In</button>
        </a>
        
        <a href="">
            <button class="header__nav__btn_blue">Join the monent</button>
        </a>
         </div>
        </div>
        </div>
        </div>
    
    </div>
</template>
<script>
export default {
     methods: {
        toggleMenu(){
            let nav = document.querySelector('.header__nav');
             nav.classList.toggle('active');
        }
     },
}
</script>
<style scoped>
*{
    margin:0;
    padding: 0;
    box-sizing: border-box;
}
    /* header */
.header__logo img{
  width: 100%;
  max-width: 60px;
  margin-top: 16px;
}

/* контенер можно свой бахнуть */
.container{
    width: 100%;
}

.header__nav ul li{
   list-style: none;
   text-align: center;
   margin-bottom: 5px;
   /* display: inline-block; */
}
.header__nav ul{
   /* display: inline-block; */
}
.header__nav ul li a{
    font-size: 16px;
   color: rgb(190, 190, 223);
   text-decoration: none;
   transition-duration: 0.5s;
   cursor: pointer;
}
.header__nav ul li a:hover{
    border-bottom: 1px solid rgb(190, 190, 223);
    padding-bottom: 3px;
    cursor: pointer;
}

.header__nav__btn{
    display: flex;
    flex-direction: column;
    text-align: center;
}
.header__nav__btn a{
    text-decoration: none;
    margin-bottom: 10px;
    /* margin-left: 35px; */
}
.header__nav__btn a:last-child{
    text-decoration: none;
    /* margin-left: 15px; */
}

.header__nav__btn_green{
    font-size: 16px;
    cursor: pointer;
    border-radius: 10px;
    border: 1px solid rgb(148, 148, 199); 
    padding: 10px 30px;
}
.header__nav__btn_blue{
    font-size: 16px;
    cursor: pointer;
    border-radius: 10px;
    border: 1px solid rgb(164, 164, 179); 
    background-color: rgb(164, 164, 179);
    color: snow;
    padding: 10px 30px;
}
/* 
@media (min-width: 576px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... } */

/* @media (min-width: 992px) {
	.header__nav_row{
        justify-content: center;
        
    }
}  */

.header__burger{
    display: block;
    text-align: center;
    cursor: pointer;
}
.header__burger-img{
    width: 36px;
    margin-top: 0;
    transform: translate3d(0px,-12px,0);
}
.header__nav{
    /* display: block; */
    height: 100%;
    max-height: 300px;
    transition-duration: 1s;
    overflow: hidden;
}
.header__nav.active{
    /* display: none; */
        max-height: 0px;
}

.header__logo{
    width: 100%;
    margin: 0 auto;
    width: 100%;
    max-width: 60px;
    transform: translate3d(0px,-14px,0);
  }

.header__nav_row{
    background-color: rgb(24, 105, 162);
    margin-top: 0px;
    display: flex;
    justify-content: center;
    flex-direction: column;
}

@media (min-width: 600px) {
    .header__burger{
        display: none;
    }
    .header__nav_row{
        display: flex;
        justify-content: space-between;
         flex-direction: row;
         padding: 0 20px;
    }
    .container{
        padding: 0 20px;
    }
    .header__nav_row_wrapper{
        width: 85%;
        margin: 0 auto;
    }
    .header__logo{
        margin: 0;
        width: 100%;
        max-width: 60px;
        transform: translate3d(0px, -6px,0);
      }
      .header__nav ul li{
        margin-top: 10px;
        list-style: none;
        text-align:justify;
        margin-bottom: 5px;
        display: inline-block;
     }
     .header__nav ul {
        margin-top: 10px;
         display: inline-block; 
    }
     .header__nav__btn{
        margin-top: 16px;
        display: inline-block;
        flex-direction: row;
        text-align:justify;
    }

} 
@media (min-width: 768px) {
	.header__nav_row{
         padding: 0 100px;
    }
    .container{
        padding: 0 120px;
    }
    .header__nav ul li a{
       margin-left: 20px;
    }
    .header__nav__btn a{
        margin-left: 25px;
    }
    .header__nav{
    /* display: block; */
    height: 100%;
    max-height: 0px;
    transition-duration: 1s;
    overflow: hidden;
}
.header__nav.active{
    /* display: none; */
        max-height: 300px;
}
} 

/* больше 1200 */
@media (min-width: 1200px) {
    .header__logo{
        margin: 0;
      }
      .header__nav ul li a{
        margin-left: 30px;
     }
     .header__nav__btn a{
         margin-left: 35px;
     }
} 


/* header */
</style>