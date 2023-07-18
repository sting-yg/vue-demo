<template> 

  <div v-bind:id="dynamicID" v-bind:class="dynamicClass">AppID</div>
  <button :disabled="isButtonDisabled">Button</button>
  <div v-bind="objectOfAttrs">测试</div>

</template>

<script>

export default{
  data(){
    return{
      
      dynamicID: "appid",
      dynamicClass: "appclass",
      isButtonDisabled: false,

      objectOfAttrs: {
        class : "appclass",
        id : "appid"
      }
    }
  }
}

</script>

<style>

  .appclass{
    color: red;
    font-size: 30px;
  }

</style>



