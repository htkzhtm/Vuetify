<template>
  <v-container class="pa-0 fluid">
    <div class="top">
      <div>
        <h1 class="kawanime">Detective Conan</h1>
        <h2 class="subtitle">The Community of Conan fan</h2>
      </div>
    </div>
  </v-container>
</template>

<script>
import Vue from 'vue';

export default Vue.extend({
  name: 'top',
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
  font-size: 12vh;
  color: #35495e;
  letter-spacing: 3px;
}
.top h2{
  font-weight: 300;
  font-size: 48px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
</style>
