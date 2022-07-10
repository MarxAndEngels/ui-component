<template lang="">
    <div class='rel'>
          <div class="form">
    <input type="checkbox" id="checkbox4" class="checkbox" />
	<label for="checkbox4" class="label">Checkbox</label>
   </div>
   <br>
    <div class="form">
    <input type="checkbox" id="checkbox5" class="checkbox" checked />
	<label for="checkbox5" class="label">Checkbox</label>
   </div>
    <br>
    <div class="form">
    <input type="checkbox" id="checkbox6" class="checkbox" />
	<label for="checkbox6" class="label">Checkbox</label>
   </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.rel{
    position: relative;
}
    .form{
            margin-left: 100px;
        }
         .checkbox {
	position: absolute;
	left: -9999px;
}

.label {
	cursor: pointer;
	font-size: 20px;
	position: relative;
}

.label:before {
	content: '';
	background-color: rgb(211, 211, 211);
	border: 2px solid rgb(108, 108, 108);
	border-radius: 5px;
	display: inline-block;
	position: absolute;
	left: -30px;
    top: 6px;
    width: 20px;
	height: 20px;
}

.label:after {
	content: '';
    background-image: url('~static/img/free-icon-perspective-1618717.png');
    width: 16px;
    height: 16px;
	 display: inline-block;
	position: absolute; 
	 left: -28px; 
	 top: 8px; 
	transform: scale(0);
	transition: transform 0.2s linear;
}

.checkbox:checked + .label:after {
	transform: scale(1);
}
</style>