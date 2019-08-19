<template>
  <v-toolbar-items class="hidden-sm-and-down">
    <v-btn
      v-for="link in links"
      :key="link.title"
      :href="link.href"
      flat
      class="white--text"
    >
      {{ link.title }}
    </v-btn>
  </v-toolbar-items>
</template>

<script>
export default {
  props: {
    links: {
      type: Array,
      default: () => ([]),
    }
  }
}
</script>
