<template>
  <div class="bg-[#24292E] lg:h-[140vh] md:h-[300vh] sm:h-[300vh]">
    <NavbarMolecula></NavbarMolecula>
    <MainContent></MainContent>
  </div>

</template>

<script>

import NavbarMolecula from "@/components/Molecules/Navbar.vue";
import MainContent from "@/components/Organisms/MainContent/MainContent.vue";




export default {
  name: 'App',

  components: {
    MainContent,
    NavbarMolecula

  }
}
</script>

<style>

</style>
