<template>
  <div class="home">
    <Top />
    <Introduction />
    <Character />
    <ComicCarousel />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Top from '@/components/Top.vue';
import Introduction from '@/components/Introduction.vue';
import Character from '@/components/Character.vue';
import ComicCarousel from '@/components/ComicCarousel.vue';

export default Vue.extend({
  name: 'home',
  components: {
    Top,
    Introduction,
    Character,
    ComicCarousel,
  },
});
</script>
