<template>
  <v-container fluid class="pb-6">
    <h2
      class="text-xs-center font-weight-bold display-1 pb-4"
    >
      {{ title }}
    </h2>
    <slot />
  </v-container>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Title'
    }
  }
}
</script>
