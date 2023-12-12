<script>
import HeaderYugioh from './components/HeaderYugioh.vue';
import ArchetypeYugioh from './components/ArchetypeYugioh.vue';
import CardList from './components/CardList.vue';
import CardInfo from './components/CardInfo.vue';

export default {
  components: {
    HeaderYugioh,
    ArchetypeYugioh,
    CardInfo,
    CardList,
  },
};
</script>

<template>
  <HeaderYugioh></HeaderYugioh>
  <ArchetypeYugioh></ArchetypeYugioh>
  <CardInfo></CardInfo>
  <CardList></CardList>
</template>

<style scoped></style>
