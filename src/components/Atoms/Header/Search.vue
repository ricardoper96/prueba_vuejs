<template>
  <div class="flex flex-row items-center  lg:inline-flex md:inline-flex sm:hidden">
    <div class="relative">
      <div class="px-2">
        <input class="lg:w-[600px] py-1 bg-[#1C2126] rounded-xl pl-2" placeholder="Search">
      </div>
      <div class="absolute top-1 right-4">
        <img src="../../../../public/imagenes/barra-navegacion/iconsearch.png">
      </div>
    </div>
    <div>
      <icon-fix></icon-fix>
    </div>
  </div>
</template>

<script>
import IconFix from "@/components/Atoms/Header/IconFix.vue";

export default {
  name: 'SearchAtom',
  components: {IconFix}
}
</script>

<style>

</style>