<template>
  <section id="introduction">
    <h1 class="title-head">Introduction of a nice detective Conan</h1>
    <div class="layout features-container row wrap">
      <div class="flex feature-container xs12">
        <div class="layout row wrap">
          <div class="flex feature xs12 md6">
            <h2 class="sub-title">The national animation in Japan</h2>
            <p class="description">Detective Conan is one of the major animations in Japan. Anime is broadcasted every Saturday.</p>
          </div>
          <div class="flex pic hidden-sm-and-down md6">
            <img src="../assets/conan.jpeg" class="img-large">
          </div>
          <div class="flex pic xs12 hidden-md-and-up">
            <img src="../assets/conan.jpeg" class="img-small">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>



<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'introduction'
})
</script>

<style scoped>
#introduction h1{
  text-align: center;
  letter-spacing: 2px;
  font-weight: 200;
  font-size: 40px;
  color: #526488;
  word-spacing: 3px;
}

#introduction {
  margin-top: 8vh;
  margin-bottom: 6vh;
  padding-top: 5vh;
  text-align: center;
}

.sub-title {
  font-weight: 200;
  font-size: 26px;
  color: #526488;
  padding-bottom: 5px;
  word-spacing: 3px;
}

.description {
  max-width: 90%;
  font-weight: 100;
  font-size: 17px;
  color: #526488;
  margin: 20px auto auto;
  line-height: 28px;
  word-spacing: 2px;
  text-align: justify;
  text-align-last: center;
  white-space: pre-wrap;
}

.layout {
  margin-top: 20px;
}
</style>

