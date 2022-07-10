<template>
    <div>
       <div class="select__block">
     <select name="" id="sel">
        <option value="1">Слово 1312312</option>
        <option value="2">Слово 2312312</option>
        <option value="3">Слово 3123123</option>
     </select>
</div>
<br>
    <div class="select__block">
     <select name="" id="sel">
        <option value="1">Слово 1312312</option>
        <option value="2">Слово 2312312</option>
        <option value="3">Слово 3123123</option>
     </select>
</div>
<br>
    <div class="select__block">
     <select name="" id="sel">
        <option value="1">Слово 1312312</option>
        <option value="2">Слово 2312312</option>
        <option value="3">Слово 3123123</option>
     </select>
</div>

  
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
       .select__block{
        position: relative;
        margin-bottom: 10px;
        width: 170px;
       }
       .select__block::after{
        content: '';
        display: block;
        border-style: solid;
        border-width: 6px 5px 0 5px;
        border-color: rgb(150, 192, 240) transparent transparent transparent;
        position: absolute;
        top: 40%;
         right: 8px;
         pointer-events: none;
       }
       .select__block select{
        position: relative;
        display: block;
        width: 100%;
        cursor: pointer;
        background: none;
        border: 0;
        -webkit-appearance: none;
        appearance: none;
        font-size: 18px;
        border-bottom: 3px solid rgb(150, 192, 240);
        padding: 4px 12px;
        /* border-radius: 3px; */
        padding-right: 20px;
        color: rgb(111, 110, 110);
       }
       .select__block select:focus{
        outline: none;
        /* border-color: rgb(108, 108, 108); */
       }
</style>