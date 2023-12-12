<script>
export default {
  name: 'app select',
  data() {
    return {};
  },
};
</script>

<template>
  <div class="container-select">
    <select id="type" name="type" form="Archetype">
      <option value="Alien">Alien</option>
    </select>
  </div>
</template>

<style scoped>
.container-select {
  padding-left: 50px;
  padding-top: 20px;

  #type {
    padding-right: 80px;
  }
}
</style>
