<template>
  <div class=" flex flex-row justify-between items-center  bg-[#20262D] rounded-xl	 w-full h-14 " >
      <Text :message="day" :fontSize="fontSize"></Text>
      <Text :message="value" :fontSize="fontSize"></Text>


  </div>
</template>

<script>


import Text from "@/components/Atoms/Text/Text.vue";

export default {
  name: 'InfoWeek',
  components: {Text},
  data(){
    return {
      value:'215.523',
      day:'Tuesday',
      fontSize:"17.16px"
    }
  }

}
</script>
