<template>
  <div class="flex flex-row">
    <div>
      <BurgerAtom></BurgerAtom>
    </div>
    <div class="pl-6">
      <LogoAtom></LogoAtom>
    </div>
  </div>
</template>
<script>
import BurgerAtom from "@/components/Atoms/Header/Burger.vue";
import LogoAtom from "@/components/Atoms/Header/Logo.vue";

export default {
  name: 'MenuLogo',
  components: {LogoAtom, BurgerAtom}
}
</script>