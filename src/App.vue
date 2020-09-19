<template>
  <div id="app">
    <Call/>
  </div>
</template>

<script>
import Call from "@/views/Call";
export default {
  name: "App",
  components: {
    Call
  }
};
</script>

<style>
#app {
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  background: #fff;
  padding: 32px 24px;
  border-radius: 16px;
  width: 384px;
  margin-left: auto;
  margin-right: auto;
}
</style>
