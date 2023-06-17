<template>

  <div class="flex flex-col">
    <div class="flex flex-row">
      <img class="px-0.5" :src="itemMain" alt="">

      <img class="px-0.5" :src="itemCompare" alt="">
    </div>
    <div class="pt-4">
      <span class="text-white font-normal">{{itemNumber}}</span>

    </div>
  </div>

</template>

<script>


export default {
  name: 'SaleItemGraph',
  props:{
    itemMain:String,
    itemCompare:String,
    itemNumber:String
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
