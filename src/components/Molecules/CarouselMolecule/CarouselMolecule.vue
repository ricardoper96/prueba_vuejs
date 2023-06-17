<template>
  <div class="h-[555px] lg:w-[879px] md:w-[879px] sm:w-[360px] mx-10 ">
   <h1 class="font-Poppins text-white text-left p-2 pt-4 text-[36px] ">Event Galleries</h1>
   <Swiper
    :modules="modules"
    :slides-per-view="1"
    :space-between="50"
    navigation
    :pagination="{ clickable: true }"
    :scrollbar="{ draggable: true }"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
     class="swiper-pagination">
      <SwiperSlide v-for="(item,index) in list" :key="`item-download_url-${index}`">
        <img :src="item.download_url" alt="" class="rounded-2xl">
      </SwiperSlide>
      
   </Swiper>
   
  </div>

</template>

<script>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import { A11y, Navigation, Pagination, Scrollbar } from 'swiper';
  
  import axios from 'axios';
  import "swiper/css/pagination";
  import 'swiper/css';
  import 'swiper/css/navigation';
  import 'swiper/css/pagination';
  import 'swiper/css/scrollbar';


import 'swiper/css';
export default {
  components: {
    Swiper,
    SwiperSlide,
  },

  name: 'CarouselMolecule',
    data(){
      return  {
        list:[]
      }
    },
    mounted() {
      axios.get('https://picsum.photos/v2/list?page=2&limit=10')
        .then(response => {
          console.log(response.data);
          this.list=response.data
        })
        .catch(error => {
          console.error(error);
        }) 
    },

       setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      
      return {
        onSwiper,
        onSlideChange,
        modules: [Navigation, Pagination, Scrollbar, A11y],
      };
    }

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
