<template>
  <v-app dark>
    <v-app-bar
      class="grey darken-3"
      fixed
      app
      light
    >
      <v-toolbar-title> H.J. de Vriesstraat 10</v-toolbar-title>

      <v-spacer></v-spacer>
<!--
      <v-toolbar-items>
        <v-btn text>Link 1</v-btn>
        <v-btn text>Link 2</v-btn>
        <v-btn text>Link 3</v-btn>
      </v-toolbar-items> -->

    </v-app-bar>
    <v-content>
      <nuxt />
    </v-content>
    <AppFooter />
  </v-app>
</template>

<script>
import AppFooter from '~/components/AppFooter.vue'
import NavDrawer from '~/components/NavDrawer.vue'
import ToolbarNavs from '~/components/ToolbarNavs.vue'

export default {
  components: {
    AppFooter,
    NavDrawer,
    ToolbarNavs,
  },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'bubble_chart',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      menuDrawer: false,
      title: 'Plyo',
    }
  }
}
</script>
