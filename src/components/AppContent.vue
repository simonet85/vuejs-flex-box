<template>
  <div class="content">
    <p>{{ contenttitle }}</p>
  </div>
</template>

<script>
export default {
  props: {
    contenttitle: {
      type: String,
      required: true,
      default: () => "Content",
      validator: (v) => typeof v === "string",
    },
  },
};
</script>
<style lang='scss' scoped>
.content {
  flex-grow: 1;
  background: #f5f5dc;
  padding: 1rem;
  justify-content: center;
  align-items: center;
}
</style>