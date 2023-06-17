<template>
  <div class="flex flex-row">
    <div>
      <TicketAtom class="p-2" :message="Tikect1.message" :url="Tikect1.dotRojo"></TicketAtom>
      <TicketAtom class="p-2" :message="Tikect2.message" :url="Tikect2.dotAzul"></TicketAtom>
    </div>


    <div>
      <TicketAtom class="p-2" :message="Ticket3.message" :url="Ticket3.dotverde"></TicketAtom>
      <TicketAtom class="p-2" :message="Ticket4.message" :url="Ticket4.dotAmarillo"></TicketAtom>
    </div>
  </div>
</template>

<script>
  import TicketAtom from "@/components/Atoms/Ticket.vue";

  export default {
    name: 'TicketsMain',
    components: { TicketAtom},
    data(){
      return{
        Tikect1:{
          dotRojo:require('../../../public/imagenes/tabla-circular-colores/puntorojo.png'),
          message:'Ticket A'
        },
        Tikect2:{
          dotAzul:require('../../../public/imagenes/tabla-circular-colores/dotazul.png'),
          message: 'Ticket B'
        },
        Ticket3:{
          dotverde:require('../../../public/imagenes/tabla-circular-colores/dotverde.png'),
          message: 'Ticket C'
        },
        Ticket4:{
          dotAmarillo:require('../../../public/imagenes/tabla-circular-colores/dotamarilla.png'),
          message:'Ticket D'
        }
      }
    }
  }


</script>

<style>

</style>