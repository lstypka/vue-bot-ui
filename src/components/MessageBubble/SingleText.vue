<template lang="pug">
.qkb-msg-bubble-component.qkb-msg-bubble-component--single-text
  .qkb-msg-bubble-component__text <div v-html="convertToHtml()"></div>
</template>
<script>
const showdown = require('showdown');
const converter = new showdown.Converter();


export default {
  components: {
  },
  props: {
    mainData: {
      type: Object
    }
  },
  methods: {
    convertToHtml() {
      return converter.makeHtml(this.mainData.text)
    }

  }

}
</script>
