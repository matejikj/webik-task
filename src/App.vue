<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <v-tabs align-with-title>
        <v-tab to="/">Hlavni</v-tab>
        <v-tab to="/about">Dalsi</v-tab>
        <v-tab to="/one">Scitac 1</v-tab>
        <v-tab to="/two">Scitac 2</v-tab>
      </v-tabs>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'App',

  data: () => ({
    //
  })
})
</script>
