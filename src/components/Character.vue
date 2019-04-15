<template>
  <section id="character">
    <h1 class="title-head">Unique character</h1>
    <div class="layout features-container row wrap">
      <div class="container">
        <h5 class="text">Detective Conan has many distinctive characters. There is a mysterious girl and a strangely smart boy.</h5>
        <h5 class="text">By the way, these days, the characters of handsome and beautiful girls are noticeable. Especially good-looking man is topic to the woman preeminently.</h5>
        <h5 class="text">As we introduce attractive character here, please have a look!</h5>
      </div>
    </div>
  <div class="text-xs-center">
    <v-dialog
      v-model="dialog"
      width="1000"
    >
      <template v-slot:activator="{ on }">
        <v-btn
          color="blue lighten-2"
          dark
          v-on="on"
        >
          Unique Characters
        </v-btn>
      </template>

      <v-card>
        <v-card-title
          class="headline grey lighten-2"
          primary-title
        >
          Unique Characters Introduction
        </v-card-title>

    <div class="layout features-container row wrap" id="unique-character">
      <div class="content flex feature-container xs12"
        v-for="introduction in introductions"
        :key="introduction.subTitle"
      >
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

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="primary"
            flat
            @click="dialog = false"
          >
            close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
  </section>
</template>

<script>
import Vue from 'vue';

export default Vue.extend({
  name: 'character',
  data () {
    return {
      dialog: false,
      introductions: [
        {
          subTitle: "Toru Amuro",
          description: "Toru Amuro is a man working at a coffee shop called Poaro. It is handsome as it looks, and popular from women. What is characteristic is that he has several \"faces\". He is also a public security police and a black organization Bourbon. The origin of the name is Amurolay of Gundam and Toru Furuya of voice actor.",
          image: require("../assets/amuro.jpg")
        },
        {
          subTitle: "Masumi Sera",
          description: "Masumi Sera is a girl who attends the same high school as Ran Mori and Shinichi Kudo. He is good at Jeet Kune Do and boasts a fighting ability that is unbeatable to men here and there. It is popular with men because of its boyish character. The name is derived from Gundam's Masu Seira",
          image: require("../assets/sera.jpg")
        },
        {
          subTitle: "Subaru Okiya",
          description: "Subaru okiya is a university student in engineering department. This is another woman's popular character. In fact, it is disguise and the true identity is FBI Shuichi Akai. The origin of the name is Gundam's Casval rem daikun.",
          image: require("../assets/okiya.jpeg")
        },  
      ]
    }
  }
});
</script>

<style scoped>
  #character h1 {
    text-align: center;
    font-weight: 400;
    letter-spacing: 2px;
    font-size: 40px;
    color: #526488;
    word-spacing: 3px;
  }
  .container {
    width: 90%;
    margin: auto;
    padding-top: 10px;
    text-align: center;
  }

  .container h5{
    font-size: 20px;
    font-weight: 300;
    line-height: 35px;
    color: #526488;
    word-spacing: 2px;
    margin-top: 3vh;
  }

#unique-characte {
  text-align: center;
}

.sub-title {
  font-weight: 350;
  font-size: 30px;
  color: #526488;
  padding-bottom: 5px;
  word-spacing: 3px;
  text-align: center;
}

.description {
  max-width: 90%;
  font-weight: 300;
  font-size: 18px;
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
  max-width: 400px;
}

.img-large{
  max-width: 400px;
}
</style>