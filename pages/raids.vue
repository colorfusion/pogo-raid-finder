<template>
  <v-row class="mb-6">
    <v-col class="mb-6" cols="12" md="8">
      <v-row>
        <v-col v-for="n in totalItems" :key="n" cols="6" md="4">
          <v-skeleton-loader
            class="mx-auto"
            type="card-heading, card-avatar"
          ></v-skeleton-loader>
        </v-col>
      </v-row>
    </v-col>
    <v-col class="mb-6 hidden-sm-and-down" cols="4">
      <v-row>
        <v-col>
          <v-sheet class="pa-6" elevation="2">
            Filter
          </v-sheet>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      items: [],
      totalItems: 100,
    }
  },
}
</script>
