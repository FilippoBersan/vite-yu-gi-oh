<script>
import axios from 'axios';
import { store } from '../store.js';
import CardInfo from './CardInfo.vue';
export default {
  name: 'CardList',
  components: {
    CardInfo,
  },
  data() {
    return {
      store,
    };
  },
  created() {
    axios.get(store.apiURL).then((response) => {
      store.cards = response.data.data;
    });
  },
};
</script>

<template>
  <div class="container">
    <CardInfo></CardInfo>
  </div>
</template>

<style scoped lang="scss"></style>
