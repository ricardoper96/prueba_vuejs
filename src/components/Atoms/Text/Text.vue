<template>
  <div>
    <h5 v-bind="htmlProps" :class="[htmlProps?.class, 'text-white', 'p-2', 'text-' + fontSize]" >{{message}}</h5>
  </div>
</template>

<script>

import { HTMLAttributes } from 'vue';

export default {
  name: 'TextAtom',
  props: {
    message: String,
    htmlProps: HTMLAttributes,
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
