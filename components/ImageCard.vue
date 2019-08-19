<template>
  <v-flex xs12 sm6 md4>
    <v-card class="ma-2">
      <v-layout class="yellow darken-2 white--text"  row>
        <v-flex xs7>
          <v-card-title primary-title>
            <div>
              <div class="headline">{{ title }}</div>
              <div>{{ subtitle }}</div>
            </div>
          </v-card-title>
        </v-flex>
        <v-flex xs5 class="py-1">
          <v-img
            src="/demi.jpg"
            height="125px"
            contain
          ></v-img>
        </v-flex>
      </v-layout>
      <v-divider light></v-divider>
      <v-card-text class="pa-3">
        <p
          class="font-weight-medium font-italic"
        >
          {{ body_text }}
        </p>
        <span v-if="monthly">per maand</span>
      </v-card-text>
      <v-card-actions v-if="action" class="pa-3">
        <v-btn flat :href="action.href">
          {{ action.title }}
        </v-btn>
      </v-card-actions>
    </v-card>
  </v-flex>
</template>

<script>
export default {
  props: [
    'action',
    'body_text',
    'title',
    'subtitle',
  ]
}
</script>
