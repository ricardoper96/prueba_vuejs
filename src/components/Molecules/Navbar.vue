<template>
  <div class="flex flex-row  bg-[#24292E] p-2 justify-between">
    <MenuLogo></MenuLogo>
    <SearchAtom></SearchAtom>
   <NotificationAtom></NotificationAtom>
   <LoginAtom></LoginAtom>
  </div>
  <div>
    <BarAtom></BarAtom>
  </div>
</template>

<script>

import {defineComponent} from "vue";
import SearchAtom from "@/components/Atoms/Header/Search.vue";
import NotificationAtom from "@/components/Atoms/Header/notification.vue";
import LoginAtom from "@/components/Atoms/Header/Login.vue";
import MenuLogo from "@/components/Atoms/Header/MenuLogo.vue";
import BarAtom from "@/components/Atoms/Header/headerBar.vue";

export default defineComponent({
  name: 'NavbarMolecula',
  components: {BarAtom, MenuLogo, LoginAtom, NotificationAtom, SearchAtom,}
})
</script>

<style>

</style>