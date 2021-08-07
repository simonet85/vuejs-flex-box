<template>
  <header class="header">
    <h2 class="m-heading">{{ profiletitle }}</h2>
  </header>
</template>

<script>
export default {
  props: ["profiletitle"],
};
</script>

<style lang="scss" scoped>
.header {
  background: #0000ff;
  padding: 1rem;
}

.m-heading {
  font: 700;
}
</style>