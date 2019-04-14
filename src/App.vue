<template>
  <v-app>
  <v-toolbar
    fixed
    app
    clipped-right
  >
    <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
    <v-toolbar-title>Title</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <!--
        <v-btn flat to="/">Introduction</v-btn>
      -->
      <v-btn flat @click="$vuetify.goTo('#introduction', { offset: 0 })">Introduction</v-btn>
      <v-btn flat @click="$vuetify.goTo('#character', { offset: 0 })">character</v-btn>
      <v-btn flat to="/author">Author Details</v-btn>
      <v-btn flat to="/twittersearch">Twitter Search</v-btn>
    </v-toolbar-items>
  </v-toolbar>
    <v-navigation-drawer
      fixed
      v-model="drawer"
      app
    >
      <v-list dense>
        <v-list-tile @click.stop="left = !left">
          <v-list-tile-action>
            <v-icon>exit_to_app</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Open Temporary Drawer</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-navigation-drawer
      temporary
      v-model="left"
      fixed
    ></v-navigation-drawer>
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
