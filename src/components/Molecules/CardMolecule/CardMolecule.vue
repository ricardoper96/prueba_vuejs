<template>
  <div :class="{'lg:block md:block sm:hidden': showMobile, 'lg:block md:block sm:block': !showMobile}" class="bg-[#2F363D] lg:w-[422.99px] md:w-[422.99px] sm:max-w-max h-[181.68px] rounded-2xl">
    <div class="flex flex-row flex-wrap justify-between mx-10 pt-3 ">
      <Text
          :message="title"
      ></Text>
      <DropDown :title="messageDropDown"></DropDown>
      <component :is="imageComponentVue"></component>
    </div>

  </div>
</template>

<script>


import DropDown from "@/components/Atoms/DropDown/DropDown.vue";
import Text from "@/components/Atoms/Text/Text.vue";

export default {
  name: 'CardModule',
  components: { Text, DropDown},
  props: {
     title:String,
     messageDropDown:String,
     imageComponentVue:{
       type:Object
     },
    showMobile:Boolean
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>