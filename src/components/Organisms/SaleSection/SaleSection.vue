<template>
  <div  class="bg-gradient-to-r from-green-basic to-green-primary h-[381.21px] w-[878.88px] rounded-2xl lg:block md:block sm:hidden">
    <SaleAtom></SaleAtom>
    <SaleGraph></SaleGraph>
  </div>
</template>

<script>



import SaleAtom from "@/components/Atoms/SaleAtom/SaleAtom.vue";
import SaleGraph from "@/components/Molecules/SaleGraph/SaleGraph.vue";

export default {
  name: 'SaleSection',
  components: {SaleGraph, SaleAtom},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
