<template>
     <div class="flex flex-col justify-center items-center">
       <img class="h-6 w-6" :src="url" alt="fdsfs">
       <Text :message="message" ></Text>


     </div>

</template>

<script>
import Text from "@/components/Atoms/Text/Text.vue";


export default {
  name: 'ItemSection',
  components:{Text},
  props: {
    message: String,
    url: String,
    fontSize: {
      type: String,
      default: '24.52px'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
