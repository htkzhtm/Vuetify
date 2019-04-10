<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex xs12>
        <v-avatar size="256px">
          <v-img
            :src="require('../assets/author.png')"
            alt="Avatar"
          ></v-img>
        </v-avatar>
      </v-flex>
      <v-card-text class="text-xs-center">
        <h1 class="category text-gray font-weight-thin mb-3">Hitomi Hatsukaze</h1>
        <p class="card-description font-weight-light">A web developer in Japan. Recently interested in using Vue.js, and Laravel for development. Get along well. Thank you.</p>
        <template v-for="(item, index) in items">

        </template>
      </v-card-text>
    </v-layout>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      items: [
        {
          title: 'Name',
          description: 'Hatsukaze Hitomi'
        },
        {
          title: 'gender',
          description: 'male'
        }
      ]
    }
  }
})
</script>

<style scoped>

</style>
