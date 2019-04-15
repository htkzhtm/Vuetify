<template>
<section id="author">
  <h1 class="title-head">Contribution for fansite</h1>
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
        <h1 class="category text-gray font-weight-thin mb-3">Hitomi Hatsukaze <a href="https://github.com/htkzhtm/Vuetify">
        <v-icon size="40px" href="https://github.com/htkzhtm/Vuetify">home</v-icon></a></h1>
        <p class="card-description font-weight-light">A web developer in Japan. Recently interested in using Vue.js, and Laravel for development. Get along well. Thank you.</p>
      </v-card-text>
    </v-layout>
  </v-container>
</section>
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
#author {
  margin-top: 20px;
}

#author h1 {
  text-align: center;
  letter-spacing: 2px;
  font-weight: 400;
  font-size: 40px;
  color: #526488;
  word-spacing: 3px;
}
</style>
