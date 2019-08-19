<template>
  <v-flex xs12 sm6 lg4 class="pa-2">
    <v-card class="black--text">
      <v-card-title primary-title class="yellow darken-2">
        <div>
          <div class="headline">{{ title }}</div>
          <span>{{ subscript }}</span>
        </div>
      </v-card-title>
      <v-card-text>
        <p
          class="mb-0 yellow--text text--darken-2 font-weight-bold display-1"
        >
          &euro; {{ price }}
        </p>
        <span v-if="monthly">per maand</span>
      </v-card-text>
      <v-list>
          <v-list-tile
            v-for="item in features"
            :key="item"
            avatar
          >
            <v-list-tile-action>
              <v-icon color="green">check</v-icon>
            </v-list-tile-action>

            <v-list-tile-content>
              <v-list-tile-title v-text="item"></v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
        </v-list>
      <v-card-actions v-if="action" class="text-xs-center">
        <v-btn
          class="black--text yellow darken-2"
          flat
          dark
          :href="action.href"
        >
          {{ action.title }}
        </v-btn>
      </v-card-actions>
    </v-card>
  </v-flex>
</template>

<script>
export default {
  props: {
    action: {
      type: Object,
      default: undefined
    },
    features: {
      type: Array,
      default: () => ([]),
    },
    monthly: {
      type: Boolean,
      default: true,
    },
    price: {
      type: String,
      default: 'bla',
    },
    title: {
      type: String,
      default: 'bla',
    },
    subscript: {
      type: String,
      default: 'fsfsf',
    },
  }
}
</script>
