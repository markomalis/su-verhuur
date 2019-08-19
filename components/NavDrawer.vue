<template>
  <v-layout
    wrap
  >
    <v-navigation-drawer
      v-model="visible"
      app
      temporary
      dark
    >
      <v-list class="pa-1">
        <v-list-tile class="px-0" >
            <img src="/plyo-logo.png" width="85px">
        </v-list-tile>
      </v-list>

      <v-list class="pt-0">
        <v-divider></v-divider>

        <v-list-tile
          v-for="item in links"
          :key="item.title"
          :href="item.href"
        >
          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </v-layout>
</template>

<script>
  export default {
    props: {
      visible: {
        type: Boolean,
        default: false,
      },
      links: {
        type: Array,
        default: () => ([])
      }
    },
    data () {
      return {
        drawer: null,
        items: [
          { title: 'Home', icon: 'dashboard' },
          { title: 'About', icon: 'question_answer' }
        ]
      }
    }
  }
</script>
