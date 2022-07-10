<template>
     <div class='rel'>
    <label for="checkbox1" class="label">
        <input type="checkbox" class="checkbox" id="checkbox1">
        <span class="check-style"></span>      checkbox
    </label>
    <br>

    <label for="checkbox2" class="label">
        <input type="checkbox" class="checkbox" checked id="checkbox2">
        <span class="check-style"></span>      checkbox active
    </label>
    <br>
    <label for="checkbox3" class="label">
        <input type="checkbox" class="checkbox" disabled id="checkbox3">
        <span class="check-style"></span>
        checkbox disabled
    </label>
</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
     *{
            box-sizing: border-box;
        }
        .rel{
            position: relative;
        }
        .label{
            display: block;
            margin-left: 26px;
            cursor: pointer;
        }
        .checkbox{
            position: absolute;
            width: 1;
            height: 1;
            overflow: hidden;
            clip: rect(0,0,0,0);
        }
        .check-style{
              position: absolute;
    width: 20px;
    height: 20px;
    border: 3px solid rgb(33, 103, 33);
    margin-left: -26px;
    margin-top: 3px;
        }
        
        .checkbox:checked + .check-style::before{
           content: '';
           width: 10px;
           height: 10px;
           background-color:rgb(33, 103, 33);
           position: absolute;
           top: 50%;
           left: 50%;
           transform: translate(-50%,-50%);
        }
        .checkbox:disabled + .check-style{
           background-color: #ccc;
        }
        .checkbox:focus + .check-style{
           box-shadow: 0 0 0 1px rgb(42, 42, 42);
        }
</style>