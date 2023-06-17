<template>
  <div class="grid lg:grid-cols-2 md:grid-cols-2 sm:grid-cols-1 pt-5    ">
      <div v-for="(card,index) in cards" :key="`item-card-${index}`">
        <div class="lg:px-2 lg:pt-6 md:px-2 md:pt-6 sm:pt-2 sm:px-2">
          <CardModule :show-mobile="card.showMobile" :title="card.title" :message-drop-down="card.messageDropDown" :image-component-vue="card.imageComponentVue"> </CardModule>

        </div>

      </div>
    <div class="px-2  ">
      <CardSpecial :titleDropDown="cardSpecial.titleDropDown"></CardSpecial>

    </div>


  </div>
</template>

<script>


import CardModule from "@/components/Molecules/CardMolecule/CardMolecule.vue";
import BarXAtom from "@/components/Atoms/BarXAtom/BarXAtom.vue";
import LineaAtom from "@/components/Atoms/Linea/LineaAtom.vue";
import LineaSecondary from "@/components/Atoms/LineaSecondary/LineaSecondary.vue";
import CardSpecial from "@/components/Molecules/CardSpecial.vue";

export default {
  name: 'CardSection',
  components: {CardSpecial, CardModule},
  data(){
    return {
      cards:[
        {
          title:'456k Pcs',
          messageDropDown:'Daily',
          imageComponentVue: BarXAtom,
          showMobile:false

        },
        {
          title:'451,509',
          messageDropDown:'This Week',
          imageComponentVue: LineaAtom,
          showMobile:false


        },
        {
          title:'$456,623',
          messageDropDown:'Monthly',
          imageComponentVue: LineaSecondary,
          showMobile:true


        },



      ],
      cardSpecial:{
        titleDropDown:'This Week'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
