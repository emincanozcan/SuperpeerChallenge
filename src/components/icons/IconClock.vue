<template>
  <svg :width="size" :height="size" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg">
    <path
      fill-rule="evenodd"
      fill="currentColor"
      clip-rule="evenodd"
      d="M12 9.75H9C8.586 9.75 8.25 9.41475 8.25 9V6C8.25 5.58525 8.586 5.25 9 5.25C9.414 5.25 9.75 5.58525 9.75 6V8.25H12C12.4148 8.25 12.75 8.58525 12.75 9C12.75 9.41475 12.4148 9.75 12 9.75ZM9 1.5C4.8645 1.5 1.5 4.8645 1.5 9C1.5 13.1355 4.8645 16.5 9 16.5C13.1355 16.5 16.5 13.1355 16.5 9C16.5 4.8645 13.1355 1.5 9 1.5Z"
    ></path>
    <mask
      id="mask0"
      mask-type="alpha"
      maskUnits="userSpaceOnUse"
      x="1"
      y="1"
      width="16"
      height="16"
    >
      <path
        fill-rule="evenodd"
        clip-rule="evenodd"
        d="M12 9.75H9C8.586 9.75 8.25 9.41475 8.25 9V6C8.25 5.58525 8.586 5.25 9 5.25C9.414 5.25 9.75 5.58525 9.75 6V8.25H12C12.4148 8.25 12.75 8.58525 12.75 9C12.75 9.41475 12.4148 9.75 12 9.75ZM9 1.5C4.8645 1.5 1.5 4.8645 1.5 9C1.5 13.1355 4.8645 16.5 9 16.5C13.1355 16.5 16.5 13.1355 16.5 9C16.5 4.8645 13.1355 1.5 9 1.5Z"
        fill="currentColor"
      ></path>
    </mask>
    <g mask="url(#mask0)"></g>
  </svg>
</template>
<script>
export default {
  name: "IconClock",
  props: ["size"]
};
</script>
