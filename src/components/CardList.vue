<script>
import axios from 'axios';
import { store } from '../store.js';
import CardInfo from './CardInfo.vue';
import ArchetypeYugioh from './ArchetypeYugioh.vue';
export default {
  name: 'CardList',
  components: {
    CardInfo,
    ArchetypeYugioh,
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
  <div class="container" v-for="card in store.cards">
    <CardInfo
      :img="card.card_images[0].image_url"
      :name="card.name"
      :archetype="card.archetype"
    />
  </div>
</template>

<style scoped lang="scss"></style>
