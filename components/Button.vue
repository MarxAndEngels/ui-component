<template>
    <div>
        
        <button type='submit' class='button'>WebDevTips 
            <span class="flare"></span>
            
            </button>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .button {
    padding: 6px 20px;
    background: #3E64FF;
    color: #ffffff;
    text-decoration: none;
    font-size: 14px;
    font-weight: 600;
    border-radius: 10px;

    position: relative; 
    overflow-x: hidden; 
    border: none;
}

.button .flare {
    position: absolute;
    top: 0;
    height: 100%;
    width: 8px;
    transform: skewX(-45deg); 
    animation: flareAnimation;
    left: -150%;
    background: linear-gradient(90deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.4));
    animation: flareAnimation 3s infinite linear; 
}

@keyframes flareAnimation {
    0% {
        left: -150%;
    }
    100% {
        left: 150%;
    }
}
</style>