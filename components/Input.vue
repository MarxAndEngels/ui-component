<template>
<div>
      <div class='container-input'>
          <input type="text" required />
        <label>E-mail</label>
    </div>
</div>
   	  
</template>
<script>
export default {
    
}
</script>
<style scoped>

.container-input {
  position:relative;
}
input{
  border: 2px solid #a7cde6;
  font-size: 16px;
  padding: 10px;
  color:black;
  border-radius:5px;
}

input:focus{
  outline:none;
}


label{
  position:absolute;
  top:20px;
  left:12px;
  transform: translateY(-50%);
  font-size: 18px;
  color:black;
  transition: all .25s linear;
  pointer-events:none;
}

input:focus ~ label,
input:not(:focus):valid ~ label{
  transform: translateY(50%);
  top:-25%;
  left:2px;
  font-size:12px;
  /* padding: 0 .3rem; */
}

</style>  
