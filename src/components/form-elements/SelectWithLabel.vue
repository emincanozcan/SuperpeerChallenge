<template>
  <div class="select-with-label">
    <label :for="id">{{label}}</label>
    <select :id="id">
      <option :value="opt.val" v-for="(opt,key) in options" :key="key">{{opt.text}}</option>
    </select>
  </div>
</template>
<script>
export default {
  name: "SelectWithLabel",
  props: ["label", "id", "options"]
};
</script>

<style lang="scss" scoped>
.select-with-label {
  display: flex;
  transition: 0.25s border;
  align-items: center;
  margin-bottom: 8px;

  label {
    flex-basis: 100px;
    flex-shrink: 0;
  }
  select {
    width: 100%;
    &:hover,
    &:focus {
      border: 1px solid var(--primary);
    }
  }
}
</style>
