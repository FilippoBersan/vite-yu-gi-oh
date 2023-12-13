<script>
export default {
  name: 'app select',

  data() {
    return {
      apiArchetype: 'https://db.ygoprodeck.com/api/v7/archetypes.php',
    };
  },
};
</script>

<template>
  <div class="container-select">
    <select id="type" name="type" form="Archetype">
      <option :value="apiArchetype">{{ apiArchetype }}</option>
    </select>
  </div>
</template>

<style scoped lang="scss">
.container-select {
  padding-left: 50px;
  padding-top: 20px;

  #type {
    padding-right: 80px;
  }
}
</style>
