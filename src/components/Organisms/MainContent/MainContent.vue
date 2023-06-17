<template>
 <div class="flex flex-row flex-wrap justify-evenly">
   <div class="pt-3">
     <SectionMain></SectionMain>
     <CardSection></CardSection>


   </div>
   <div class="  lg:pt-3 md:pt-3 sm:pt-0">
     <SaleSection></SaleSection>
     <CarouselMolecule></CarouselMolecule>


   </div>




 </div>





</template>

<script>





import SectionMain from "@/components/Organisms/SectionMain/SectionMain.vue";
import SaleSection from "@/components/Organisms/SaleSection/SaleSection.vue";
import CardSection from "@/components/Organisms/CardsSection/CardSection.vue";
import CarouselMolecule from "@/components/Molecules/CarouselMolecule/CarouselMolecule.vue";

export default {
  name: 'MainContent',
  components: {CarouselMolecule, CardSection, SaleSection, SectionMain},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
