<template lang="pug">
.qkb-msg-bubble-component.qkb-msg-bubble-component--single-text
  .qkb-msg-bubble-component__text <div v-html="mainData.text"></div>
</template>
<script>
export default {
  props: {
    mainData: {
      type: Object
    }
  }
}
</script>
