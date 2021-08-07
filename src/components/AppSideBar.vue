<template>
  <div class="sidebar">
    <p>{{ sidebartitle }}</p>
  </div>
</template>

<script>
export default {
  props: ["sidebartitle"],
};
</script>

<style lang='scss' scoped>
.sidebar {
  background: #6495ed;
  border-right: 5px dashed blueviolet;
  padding: 1rem;
}
</style>