<template>
  <v-app>
  <v-toolbar
    fixed
    app
    clipped-right
  >
    <v-toolbar-title>Detective Conan</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <!--
        <v-btn flat to="/">Introduction</v-btn>
      -->
      <v-btn flat @click="$vuetify.goTo('#introduction', { offset: 0 })">Introduction</v-btn>
      <v-btn flat @click="$vuetify.goTo('#character', { offset: 0 })">character</v-btn>
      <v-btn flat to="/author">Author Details</v-btn>
    </v-toolbar-items>
  </v-toolbar>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      drawer: true,
      left: null
    };
  },
  props: {
    source: String
  }
}
</script>
