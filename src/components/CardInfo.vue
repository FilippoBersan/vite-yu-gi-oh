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

      <div class="text">
        <h3>{{ name }}</h3>
        <p>{{ archetype }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.container-cards {
  display: flex;
  text-align: center;
  flex-direction: column;
  background-color: rgb(152, 109, 30);
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
