<template>
  <header>
    <p class="call-with">Call with</p>
    <h3 class="h3-title">{{withName}}</h3>
  </header>
</template>
<script>
export default {
  name: "CallTitle",
  props: ["withName"]
};
</script> 
<style lang="scss" scoped>
.call-with {
  color: var(--primary);
  font-size: 13px;
  text-align: center;
  margin-bottom: 4px;
}
.h3-title {
  color: var(--grey90);
  font-size: 24px;
  font-weight: 700;
  text-align: center;
}
</style>