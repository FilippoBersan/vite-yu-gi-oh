<script>
export default {
  name: 'Card info',
  props: ['img', 'name', 'archetype'],
};
</script>

<template>
  <div class="container-cards">
    <div>
      <img :src="img" alt="name" />

      <h3>{{ name }}</h3>
      <strong>{{ archetype }}</strong>
    </div>
  </div>
</template>

<style scoped lang="scss">
.container-cards {
  display: flex;
  flex-direction: column;
  background-color: orange;
  width: 200px;
  height: 400px;

  h3 {
    color: azure;
  }

  img {
    height: 280px;
    width: 100%;
  }
}
</style>
