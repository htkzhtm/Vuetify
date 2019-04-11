<template>
  <div class="home">
    <Top />
    <Introduction />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Top from '@/components/Top.vue'; // @ is an alias to /src
import Introduction from '@/components/Introduction.vue';

export default Vue.extend({
  name: 'home',
  components: {
    Top,
    Introduction,
  },
});
</script>
