<template>
  <div class="video-preview">
    <img :src="imgUrl" alt="video-preview-image">
    <div class="video-preview-buttons">
      <button class="video-preview-buttons-button">
        <icon-mic size="20"/>
      </button>
      <button class="video-preview-buttons-button">
        <icon-cam size="20"/>
      </button>
      <button class="video-preview-buttons-button">
        <icon-settings size="20"/>
      </button>
    </div>
  </div>
</template>
<script>
import IconMic from "@/components/icons/IconMic";
import IconCam from "@/components/icons/IconCam";
import IconSettings from "@/components/icons/IconSettings";
export default {
  name: "VideoPreview",
  components: {
    IconMic,
    IconCam,
    IconSettings
  },
  props: ["imgUrl"]
};
</script>

<style lang="scss" scoped>
.video-preview {
  overflow: hidden;
  border-radius: 8px;
  height: 192px;
  position: relative;

  img {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }

  &-buttons {
    position: absolute;
    bottom: 12px;
    left: 50%;
    width: 100%;
    display: flex;
    justify-content: center;
    transform: translateX(-50%);

    &-button {
      border: none;
      border-radius: 9999px;
      height: 48px;
      width: 48px;
      line-height: 1;
      margin: 0 6px;
      background: var(--grey10);
      transition: 0.35s background;
      &:hover {
        background: var(--grey40);
      }
    }
  }
}
</style>
