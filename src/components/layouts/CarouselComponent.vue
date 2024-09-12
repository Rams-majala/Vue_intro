<template>
    <v-carousel
    cycle
    delimiter-icon="mdi-star"
    hide-delimiter-background
    show-arrows-on-hover
    >
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        :reverse-transition="transition"
        transition="fade-transition"
      > 
      <h1 class="white--text">Welcome to Hello World</h1>
      </v-carousel-item>
    </v-carousel>
</template>
<script>
  export default {
    name: 'CarouselComponent',
    data () {
      return {
        transition: 'fade-transition',
        items: [
          {
            src: require('@/assets/images/artempodrez.jpg'),
          },
          {
            src: require('@/assets/images/holding.jpg'),
          },
          {
            src: require('@/assets/images/trans_computer.jpg'),
          },
          {
            src: require('@/assets/images/man_computer.jpg'),
          },
        ],
      }
    },
  }
</script>