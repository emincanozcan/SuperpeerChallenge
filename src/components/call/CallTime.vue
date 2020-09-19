<template>
  <div class="call-time">
    <div class="call-time-box">
      <div class="call-time-box-column">
        <icon-calendar size="18"/>
        <span>{{date}}</span>
      </div>
      <div class="call-time-box-column">
        <icon-clock size="18"/>
        <span>{{startingAt}} - {{endingAt}}</span>
      </div>
    </div>
    <p class="call-time-timezone">Timezone: {{timezone}}</p>
  </div>
</template>
<script>
import IconCalendar from "@/components/icons/IconCalendar";
import IconClock from "@/components/icons/IconClock";
export default {
  name: "CallTime",
  components: { IconCalendar, IconClock },
  props: ["date", "startingAt", "endingAt", "timezone"]
};
</script>
<style lang="scss" scoped>
.call-time {
  margin: 16px 16px 24px 16px;

  &-box {
    border-radius: 8px;
    padding: 16px;
    border: 1px solid var(--borderColor);
    display: flex;
    align-items: center;
    justify-content: space-between;

    &-column {
      display: flex;
      align-items: center;

      span {
        margin-left: 9.5px;
        font-size: 13px;
      }

      svg {
        color: var(--primary);
      }
    }
  }

  &-timezone {
    color: var(--grey80);
    font-size: 13px;
    text-align: center;
    margin-top: 8px;
  }
}
</style>
