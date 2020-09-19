<template>
  <div>
    <call-title with-name="Niloya Kayıkçı"/>
    <call-time
      date="7 Oct, Weds"
      starting-at="10:15AM"
      ending-at="10:30AM"
      timezone="Timezone: Europe/Amsterdam"
    />
    <video-preview
      img-url="https://s3-alpha-sig.figma.com/img/80b2/c8b9/db05a73b5f7cb33be5906f4d71d57593?Expires=1601251200&Signature=EMlA3~QQkzTQjy7TmQsjtT2CSZq0P8owfYw5z7m48j2niJ3bi6L8LPqT6iCw-i386tYZtHYQyvG3nWwBB1x8pwRWzIkU3giMNTlv3LMzGG7Hs5gbN9vb1OczBCL04-yykkOLgJK35Y2t~uNQJlmKOfnhrjR6cQVEEQ-fbK9KKsc96j3T65blH6nTd0f6aDm-qZ87EZDWnlsLsLeBwvIW6ORahfR85KtWhOZ4nd1~~QHkt5z0JLs7KoCVep5NQEApnh8ogdsb3PQfW4JG6xTNzd7qmYaBabqHmN3pb7T5sC5PAXvX4cmH6Rq-4qGCfUq~kV4Ebfj4iJ5sNA06ZU4lzw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
    />
    <input-with-person-icon name="Adem İlter"></input-with-person-icon>
    <settings/>
    <button class="primary join-call">Join Call</button>
  </div>
</template>
<script>
import CallTitle from "@/components/call/CallTitle";
import CallTime from "@/components/call/CallTime";
import VideoPreview from "@/components/call/VideoPreview";
import Settings from "@/components/call/Settings";
import InputWithPersonIcon from "@/components/form-elements/InputWithPersonIcon";
export default {
  name: "call",
  components: {
    CallTitle,
    CallTime,
    VideoPreview,
    Settings,
    InputWithPersonIcon
  }
};
</script>
<style>
.join-call {
  margin-top: 16px;
}
</style>
