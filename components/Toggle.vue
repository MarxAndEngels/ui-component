<template>
    <div>
        <div id="nav-icon3" @click='openMenu()'>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
</div>
    </div>
</template>
<script>
export default {
    methods:{
           openMenu(){
            let menu = document.querySelector('#nav-icon3');
            menu.classList.toggle('open');
        }
    }
}
</script>
<style scoped>
    
#nav-icon3 {
    width: 26px;
    height: 22px;
    position: relative;
    margin: 10px;
    transform: rotate(0deg);
    transition: .5s ease-in-out;
    cursor: pointer;
} 
#nav-icon3 span {
    display: block;
    position: absolute;
    height: 4px;
    width: 100%;
    background: black;
    border-radius: 9px;
    left: 0;
    transform: rotate(0deg);
    transition: .75s ease-in-out;
        opacity: 1;
}
#nav-icon3 span:nth-child(1) {
    top: 0px;
}
#nav-icon3 span:nth-child(2),
#nav-icon3 span:nth-child(3) {
    top: 10px;
}
#nav-icon3 span:nth-child(4) {
    top: 20px;
}
#nav-icon3.open span:nth-child(1) {
    top: 18px;
    width: 0%;
    left: 50%;
    opacity: 0.5;
}
#nav-icon3.open span:nth-child(2) {
    transform: rotate(45deg);
        opacity: 0.5;
}
#nav-icon3.open span:nth-child(3) {
    transform: rotate(-45deg);
        opacity: 0.5;
}
#nav-icon3.open span:nth-child(4) {
    top: 18px;
    width: 0%;
    left: 50%;
    opacity: 0.5;
}
</style>