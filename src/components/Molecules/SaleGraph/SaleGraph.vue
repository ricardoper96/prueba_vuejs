<template>
  <div>
    <div class="flex flex-row justify-evenly items-baseline">

      <img  alt="" src="../../../assets/imagenes/tabla-grafica/paginator_1.png">

      <div v-for="(itemGraph,index) in itemsGraph" :key="`item-graph-${index}}`">
        <SaleItemGraph :item-number="itemGraph.number" :item-compare="itemGraph.itemCompare" :item-main="itemGraph.itemMain"></SaleItemGraph>
      </div>
      <img alt="" src="../../../assets/imagenes/tabla-grafica/paginator_2.png">

    </div>
  </div>

</template>

<script>


import SaleItemGraph from "@/components/Atoms/SaleItemGraph/SaleItemGraph.vue";

export default {
  name: 'SaleGraph',
  components: {SaleItemGraph},
  data(){
    return {
      itemsGraph:[
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/01.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/02.png'),
          number:"06"
        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/03.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/04.png'),
          number:"07"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/05.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/06.png'),
          number:"08"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/07.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/08.png'),
          number:"09"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/09.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/10.png'),
          number:"10"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/11.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/12.png'),
          number:"11"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/13.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/14.png'),
          number:"12"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/15.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/16.png'),
          number:"13"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/17.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/18.png'),
          number:"14"

        },
        {
          itemMain:require('../../../assets/imagenes/tabla-grafica/19.png'),
          itemCompare:require('../../../assets/imagenes/tabla-grafica/20.png'),
          number:"15"

        },

      ]
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
