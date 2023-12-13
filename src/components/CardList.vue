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

    axios.get(store.apiURL).then((resp) => {
      store.imgCards = resp.data.card_images;
    });
  },
};
</script>

<template>
  <div class="container" v-for="card in store.cards">
    <CardInfo
      :img="card.card_images[0].image_url"
      :name="card.name"
      :archetype="card.archetype"
    />
  </div>
</template>

<style scoped lang="scss"></style>
