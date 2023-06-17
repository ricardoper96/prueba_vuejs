<template>
  <div class="flex flex-row pt-10 pl-10">

    <div class="flex flex-row justify-evenly">

      <div class="px-4" v-for="(day, index) in dataDays" :key="`data-${day.textMonth}-${index}`">
        <ItemCalendar :itemFill="day.textMonth" :urlImg="day.urlImg"></ItemCalendar>
      </div>

    </div>
  </div>
</template>

<script>



import ItemCalendar from "@/components/Atoms/ItemCalendar/ItemCalendar.vue";

export default {
  name: 'CalendarMolecule',
  components: {ItemCalendar},
  data(){
    return {
      dataDays:[
          {
      textMonth:'S',
          urlImg:require('../../../assets/imagenes/tabla-circular/3.png')
    },
          {
            textMonth:'M',
                urlImg: require('../../../assets/imagenes/tabla-circular/2.png')
          },
          {
            textMonth:'T',
                urlImg: require('../../../assets/imagenes/tabla-circular/4.png')

          },
          {
            textMonth:'W',
                urlImg: require('../../../assets/imagenes/tabla-circular/5.png')

          },
          {
            textMonth:'T',
                urlImg: require('../../../assets/imagenes/tabla-circular/6.png')

          },
          {
            textMonth:'F',
                urlImg: require('../../../assets/imagenes/tabla-circular/7.png')
          },
          {
            textMonth:'S',
                urlImg: require('../../../assets/imagenes/tabla-circular/2.png')
          }
      ],

    }
  }


}
</script>
