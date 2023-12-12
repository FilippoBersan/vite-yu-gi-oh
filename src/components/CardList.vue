<script>
import axios from 'axios';
import CardInfo from './CardInfo.vue';
export default {
  name: 'CardList',
  components: {
    CardInfo,
  },
  data() {
    return {
      cards: [],
      apiURL: 'https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0',
    };
  },
  created() {
    axios.get(this.apiURL).then((response) => {
      this.cards = response.data.data.data;
    });
  },
};
</script>

<template>
  <div class="container">
    <CardList v-for="card in cards"></CardList>
  </div>
</template>

<style scoped lang="scss"></style>
