<template>
  <div class="home">
    <Top />
    <Introduction />
    <Character />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Top from '@/components/Top.vue'; // @ is an alias to /src
import Introduction from '@/components/Introduction.vue';
import Character from '@/components/Character.vue';

export default Vue.extend({
  name: 'home',
  components: {
    Top,
    Introduction,
    Character,
  },
});
</script>
