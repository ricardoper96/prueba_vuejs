<template>
  <div class="flex flex-row items-center  ">
   <div class="px-1">
     <p class="leading-[22.06px] text-[14.71px] text-[#B7B7B7]">{{title}}</p>

   </div>
    <div class="px-1">
      <img src="../../../assets/imagenes/barra-navegacion/arrow1.png">
    </div>
  </div>
</template>

<script>


export default {
  name: 'DropDown',
  components: {},
  props: {
    title: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
