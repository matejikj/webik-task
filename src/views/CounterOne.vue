<template>
  <v-container>
    <h1>Odcitac</h1>
    <br/>
    <br/>
    <v-row class="text-center">
      <v-btn
        class="mx-2"
        fab
        dark
        color="red"
        v-on:click="decrement()"
      >
        {{ count }}
      </v-btn>
    </v-row>
    <v-row class="text-center">
    </v-row>
    <v-row class="text-center">
    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home',

  computed: {
    count () {
      return this.$store.state.count
    }
  },
  methods: {
    decrement () {
      this.$store.commit('decrement')
      console.log(this.$store.state.count)
    }
  }
})
</script>
