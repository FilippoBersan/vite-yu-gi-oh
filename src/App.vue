<script>
import axios from 'axios';
import HeaderYugioh from './components/HeaderYugioh.vue';
import ArchetypeYugioh from './components/ArchetypeYugioh.vue';

export default {
  components: {
    HeaderYugioh,
    ArchetypeYugioh,
  },
  data() {
    return {
      cards: [],
      apiURL: 'https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0',
    };
  },
  created() {
    axios.get(this.apiURL).then((response) => {
      this.cards = response.data.data;
      console.log(this.cards);
    });
  },
};
</script>

<template>
  <HeaderYugioh></HeaderYugioh>
  <ArchetypeYugioh></ArchetypeYugioh>
</template>

<style scoped></style>
