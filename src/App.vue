<template>
  <v-app>
  <v-toolbar>
    <v-toolbar-side-icon></v-toolbar-side-icon>
    <v-toolbar-title>Title</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat @click="show">Introduction</v-btn>
      <v-btn flat>Author Details</v-btn>
      <v-btn flat>Contacts</v-btn>
    </v-toolbar-items>
  </v-toolbar>

    <v-content>
      <HelloWorld/>
      <router-link to="author">author</router-link>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data () {
    return {
      //
    }
  }
}
</script>
