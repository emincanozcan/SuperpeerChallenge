<template>
  <div class="input-with-person-icon">
    <icon-person size="24"/>
    <input :value="name">
  </div>
</template>
<script>
import IconPerson from "@/components/icons/IconPerson";
export default {
  name: "InputWithPersonIcon",
  components: { IconPerson },
  props: ["name"]
};
</script>
<style lang="scss" scoped>
.input-with-person-icon {
  position: relative;
  margin-top: 16px;
  svg {
    color: var(--primary);
    position: absolute;
    left: 16px;
    top: 50%;
    transform: translatey(-50%);
  }

  input {
    border-radius: 8px;
    border: 1px solid var(--borderColor);
    width: 100%;
    padding: 15px 6px 15px 46px;
    transition: 0.25s border;

    &:hover,
    &:focus {
      border: 1px solid var(--primary);
    }
  }
}
</style>
