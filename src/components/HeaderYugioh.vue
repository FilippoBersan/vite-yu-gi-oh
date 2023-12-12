<script>
export default {
  name: 'app header',
  data() {
    return {
      logo: './public/logo.png',
    };
  },
};
</script>

<template>
  <header>
    <div class="container-header">
      <img :src="logo" alt="" />
      <h1>Yu-Gi-Oh Api</h1>
    </div>
  </header>
</template>

<style scoped>
.container-header {
  display: flex;
  gap: 20px;
  height: 50px;
  background-color: rgb(198, 198, 198);

  h1 {
    align-self: center;
  }
}
</style>
