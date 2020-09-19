<template>
  <div class="outline-button-with-label">
    <label>{{label}}</label>
    <button class="outline">{{text}}</button>
  </div>
</template>
<script>
export default {
  name: "OutlineButtonWithLabel",
  props: ["label", "id", "text"]
};
</script>
<style lang="scss" scoped>
.outline-button-with-label {
  display: flex;
  align-items: center;
  margin-bottom: 8px;

  label {
    flex-basis: 100px;
    flex-shrink: 0;
  }

  select,
  button {
    width: 100%;
  }
}
</style>

