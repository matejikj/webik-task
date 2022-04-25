<template>
  <v-container>
    <h1>Hlavni stranka</h1>
    <br/>
    <br/>
    <v-row>
      <v-btn v-on:click="text = ''">
        Smaz
      </v-btn>
    </v-row>
    <v-row>
      <v-text-field v-model="text"></v-text-field>
    </v-row>
    <v-row>
      <h2>{{ text }}</h2>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home',

  data () {
    return {
      text: ''
    }
  }
})
</script>
