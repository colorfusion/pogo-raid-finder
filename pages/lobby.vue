<template>
  <v-row class="mb-6">
    <v-col class="mb-6" cols="12" md="8">
      <v-row>
        <v-col cols="12">
          <v-skeleton-loader type="image" height="8em" boilerplate />
        </v-col>
      </v-row>
      <v-row>
        <v-col v-for="n in 2" :key="n" cols="6">
          <v-skeleton-loader type="image" height="4em" boilerplate />
        </v-col>
      </v-row>
      <v-row v-for="n in 6" :key="n">
        <v-col cols="12" class="pa-1">
          <v-skeleton-loader
            type="list-item-avatar-three-line"
            height="5em"
            boilerplate="true"
          />
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>
