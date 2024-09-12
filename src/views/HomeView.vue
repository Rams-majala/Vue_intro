<template>
  <div>
  <CarouselComponent />
  <v-img :src="image">
    <v-container>

    <v-card class="pa-16 col-6 transparent">
      <h1>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo, suscipit laboriosam, quis minima quas ad, earum consequatur saepe aliquid quaerat nostrum. Enim voluptate minus eius, quibusdam expedita repellat itaque! Laudantium?</h1>
    </v-card>
    </v-container>
  </v-img>
  </div>
</template>

<script>
import CarouselComponent from '@/components/layouts/CarouselComponent.vue'


  export default {
    name: 'HomeView',

    components: {
        CarouselComponent
      
    },
    data(){
      return{
        image: require('@/assets/images/holding.jpg'),

      }
    }
  }
</script>
