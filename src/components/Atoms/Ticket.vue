<template>
  <div class="flex flex-row flex-wrap">
    <img :src="url"/>
    <p class="text-white ml-2">{{message}}</p>
  </div>
</template>

<script>
export default {
  name: 'TicketAtom',
  props:{
    message: String,
    url: String
  }
}
</script>

<style>

</style>