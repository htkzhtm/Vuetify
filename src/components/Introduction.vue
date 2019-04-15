<template>
  <section id="introduction">
    <h1 class="title-head">Introduction of a nice detective Conan</h1>
    <div class="layout features-container row wrap">
      <div class="content flex feature-container xs12"
        v-for="(introduction, index) in introductions"
        :key="introduction.subTitle"
      >
        <div v-if="index%2 == 0">
          <div class="layout row wrap">
            <div class="flex feature xs12 md6">
              <h2 class="sub-title">{{ introduction.subTitle }}</h2>
              <p class="description">{{ introduction.description }}</p>
            </div>
            <div class="flex pic hidden-sm-and-down md6">
              <img :src="introduction.image" class="img-large">
            </div>
            <div class="flex pic xs12 hidden-md-and-up">
              <img :src="introduction.image" class="img-small">
            </div>
          </div>
        </div>
        <div v-if="index%2 == 1">
          <div class="layout row wrap">
            <div class="flex pic hidden-sm-and-down md6">
              <img :src="introduction.image" class="img-large">
            </div>
            <div class="flex feature xs12 md6">
              <h2 class="sub-title">{{ introduction.subTitle }}</h2>
              <p class="description">{{ introduction.description }}</p>
            </div>
            <div class="flex pic xs12 hidden-md-and-up">
              <img :src="introduction.image" class="img-small">
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>



<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'introduction',
  data () {
    return {
      introductions: [
        {
          subTitle: "The national animation in Japan",
          description: "Detective Conan is one of the major animations in Japan. Anime is broadcasted every Saturday.",
          image: require("../assets/conan.jpeg")
        },
        {
          subTitle: "The main character is a high school student with a shrinking body!?",
          description: "The true name of Edogawa Conan is Kudo Shinichi. He was taken APTX4869 by somebody and his body shrank. Such is the story he solves many cases.",
          image: require("../assets/shinichi.jpg")
        },
        {
          subTitle: "Love and Comedy",
          description: "This work not only solves the case, but also specializes in love and codedy. Therefore it is also supported by women.",
          image: require("../assets/ran.jpg")
        },  
      ]
    }
  }
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

.content {
  margin-top: 20px;
}

.img-small{
  max-width: 500px;
}

.img-large{
  max-width: 500px;
}

</style>

