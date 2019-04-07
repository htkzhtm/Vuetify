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
            class="my-3"
            contain
            height="200"
            alt="Avatar"
          ></v-img>
        </v-avatar>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    
})
</script>

<style scoped>

</style>
