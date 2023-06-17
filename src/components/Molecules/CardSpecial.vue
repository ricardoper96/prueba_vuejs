<template>
  <div class="bg-[#2F363D]  lg:w-[422.99px] md:w-[422.99px] sm:w-full h-[181.68px] rounded-2xl lg:mb-28 md:mb-28 lg:mt-6 md:mt-6 sm:mt-1.5 sm:mb-10" >
    <div>
      <div class="pt-1 lg:block md:block sm:hidden">
        <DropDown class="justify-end mr-8 mt-6" :title="titleDropDown"></DropDown>
      </div>
      <div class="relative    left-8">
        <GraphicColors></GraphicColors>
      </div>
      <div class="relative lg:block md:block sm:hidden left-44 top-4 p-4">
        <TicketsMain></TicketsMain>
      </div>
    </div>
  </div>
</template>

<script>

import {defineComponent} from "vue";
import TicketsMain from "@/components/Molecules/TicketsMain.vue";
import GraphicColors from "@/components/Atoms/CircleColors.vue";
import DropDown from "@/components/Atoms/DropDown/DropDown.vue";

export default defineComponent({
  components: {DropDown, GraphicColors, TicketsMain},
  props:{
    titleDropDown: String
  }

})
</script>

<style>

</style>