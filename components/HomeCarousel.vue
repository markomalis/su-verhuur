<template>
  <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: '/img1.jpg'
          },
          {
            src: '/img2.jpg'
          },
          {
            src: '/img3.jpg'
          },
          {
            src: '/img4.jpg'
          },
          {
            src: '/img5.jpg'
          },
          {
            src: '/img6.jpg'
          },
        ]
      }
    }
  }
</script>
