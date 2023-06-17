<template>

  <div class="px-1 relative ">
    <p class="absolute text-gray-400 top-44 ">{{itemFill}}</p>
    <div class="">

      <img class="absolute  " src="../../../assets/imagenes/tabla-circular/01.png" alt="">
      <img class="absolute bottom-[-160px]"  :src="urlImg" alt="">
    </div>


  </div>
  
</template>

<script>



export default {
  name: 'ItemCalendar',
  props:{
    itemFill:String,
    urlImg: String
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
