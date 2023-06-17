<template>
  <div class="bg-[#272E35] lg:h-[606.76px] md:h-[606.76px]  lg:w-[878.88px] w-auto   sm:h-[580px] rounded-2xl">
    <div class="flex flex-row flex-wrap justify-between mx-10 pt-3 relative">
      <Text
          message="Best Selling"
      ></Text>
      <DropDown title="This week"></DropDown>
    </div>
    <div class="mx-10">
      <InfoWeek></InfoWeek>

    </div>




    <div class="grid   lg:grid-cols-2 md:grid-cols-2  gap-6 pt-16">

      <div class=" flex flex-col h-96">
        <div class="relative">
          <div class="circle  ">
            <CircleGrafic></CircleGrafic>
          </div>
          <div class="flex flex-row flex-wrap pl-2 pt-10 lg:justify-evenly md:justify-start">
            <ItemSection :message="color.message" :url="color.colorBase"></ItemSection>
            <ItemSection :message="color2.message" :url="color2.colorBase"></ItemSection>
            <ItemSection :message="color3.message" :url="color3.colorBase"></ItemSection>


          </div>
        </div>

      </div>
      <div>
        <div class="calendar relative lg:block md:block sm:hidden">
          <CalendarMolecule></CalendarMolecule>
        </div>
      </div>
    </div>



  </div>
</template>

<script>


import Text from "@/components/Atoms/Text/Text.vue";
import DropDown from "@/components/Atoms/DropDown/DropDown.vue";
import InfoWeek from "@/components/Molecules/InfoWeek/InfoWeek.vue";
import CircleGrafic from "@/components/Molecules/CircleGrafic/CircleGrafic.vue";
import ItemSection from "@/components/Molecules/ItemSection/ItemSection.vue";

import CalendarMolecule from "@/components/Molecules/Calendar/Calendar.vue";

export default {
  name: 'SectionMain',
  components: {CalendarMolecule, ItemSection, CircleGrafic, InfoWeek, DropDown, Text},
  data(){
    return {
      color:{
        colorBase:require('../../../assets/imagenes/tabla-circular/color_base.png'),
        message:'Movies Ticket'

      },
      color2:{
        colorBase:require('../../../assets/imagenes/tabla-circular/color_base_2.png'),
        message:'Music Ticket'

      },
      color3:{
        colorBase:require('../../../assets/imagenes/tabla-circular/color_base_3.png'),
        message:'Football Ticket'

      }
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
