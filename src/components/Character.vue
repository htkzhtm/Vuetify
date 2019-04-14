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
  </section>
</template>

<script>
import Vue from 'vue';

export default Vue.extend({
  name: 'character',
});
</script>

<style scoped>
  #character h1 {
    text-align: center;
    font-weight: 300;
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
    font-weight: 200;
    line-height: 35px;
    color: #526488;
    word-spacing: 2px;
    margin-top: 3vh;
  }
</style>