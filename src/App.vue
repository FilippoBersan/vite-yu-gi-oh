<script>
import HeaderYugioh from './components/HeaderYugioh.vue';
import ArchetypeYugioh from './components/ArchetypeYugioh.vue';
import CardList from './components/CardList.vue';
import CardInfo from './components/CardInfo.vue';
import CardFound from './components/CardFound.vue';

export default {
  components: {
    HeaderYugioh,
    ArchetypeYugioh,
    CardInfo,
    CardList,
    CardFound,
  },
};
</script>

<template>
  <HeaderYugioh></HeaderYugioh>
  <ArchetypeYugioh></ArchetypeYugioh>

  <div class="container-card">
    <CardFound />
    <CardList></CardList>
  </div>
</template>

<style scoped>
.container-card {
  display: flex;
  justify-content: space-around;
  gap: 1.25rem;
  flex-wrap: wrap;
  margin: 0 auto;
  background-color: aliceblue;
  margin-top: 20px;
  width: 80%;
  padding: 30px;
}
</style>
