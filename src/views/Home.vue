<template>
  <div class="home">
    <Top />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Top from '@/components/Top.vue'; // @ is an alias to /src

export default Vue.extend({
  name: 'home',
  components: {
    Top,
  },
});
</script>
