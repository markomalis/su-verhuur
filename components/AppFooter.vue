<template>
  <v-footer
    dark
    height="auto"
  >
    <v-flex
      text-center
      xs12
    >
      {{ new Date().getFullYear() }} — <strong> H.J. de Vriesstraat 10</strong>
    </v-flex>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'fa fa-facebook',
        'fa fa-twitter',
        'fa fa-linkedin',
        'fa fa-instagram'
      ]
    })
  }
</script>
