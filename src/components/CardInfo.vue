<script>
export default {
  name: 'Card info',
};
</script>

<template>
  <div class="container-main">
    <div class="container-cards">
      <div>img</div>
      <h3>{{}}</h3>
      <p>tipo</p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.container-main {
  display: flex;
  margin: 0 auto;
  background-color: aliceblue;
  margin-top: 20px;
  width: 80%;
}
.container-cards {
  display: flex;
  flex-direction: column;
}
</style>
