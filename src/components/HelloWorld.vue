<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <div class="top">
        <div>
          <h1 class="kawanime">Detective Conan</h1>
          <h2 class="subtitle">The Community of Conan fan</h2>
        </div>
      </div>
    </v-layout>
  </v-container>
</template>

<script>
import Vue from 'vue';

export default Vue.extend({
});
</script>

<style scoped>
.top {
    display: flex;
    -webkit-box-pack: center;
    justify-content: center;
    align-items: center;
    width: 100%;
    background-image: url(https://i.imgur.com/RsrihUO.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 70vh;
    padding-bottom: 10vh;
}
.top h1{
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 200;
  font-size: 10vh;
  color: #35495e;
  letter-spacing: 3px;
}
.top h2{
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
</style>
