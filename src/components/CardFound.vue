<script>
import { store } from '../store';
export default {
  name: 'CardFound',
  data() {
    return {
      store,
    };
  },
};
</script>

<template>
  <div class="container">
    <p>Found {{ store.cards.length }} cards!</p>
  </div>
</template>

<style scoped lang="scss">
.container {
  background-color: rgb(78, 78, 78);
  width: 100%;

  p {
    color: aliceblue;
    text-align: center;
  }
}
</style>
