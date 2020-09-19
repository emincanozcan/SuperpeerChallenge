<template>
  <div class="settings">
    <select-with-label id="select-with-label-camera" label="Camera" :options="camOptions"></select-with-label>
    <select-with-label id="select-with-label-speaker" label="Speaker" :options="speakerOptions"></select-with-label>
    <select-with-label id="select-with-label-microphone" label="Microphone" :options="micOptions"></select-with-label>
    <outline-button-with-label label="Sound Test" text="Play Sound"/>
  </div>
</template>
<script>
import SelectWithLabel from "@/components/form-elements/SelectWithLabel";
import OutlineButtonWithLabel from "@/components/form-elements/OutlineButtonWithLabel";
export default {
  name: "Settings",
  components: {
    SelectWithLabel,
    OutlineButtonWithLabel
  },
  data() {
    return {
      // dummy data
      camOptions: [
        { val: "cam1", text: "Facetime HD Camera" },
        { val: "cam2", text: "Logitech Webcam" }
      ],
      speakerOptions: [
        { val: "speaker1", text: "Built-in Output (Headphones)" },
        { val: "speaker2", text: "Built-in Output (Headphones) 2" }
      ],
      micOptions: [
        { val: "mic1", text: "Built-in Microphone (More Details...)" },
        { val: "mic2", text: "Built-in Microphone (More Details...) 2" }
      ]
    };
  },
  props: ["imgUrl"]
};
</script>
<style>
.settings {
  margin-top: 24px;
}
</style>
