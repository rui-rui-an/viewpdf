<template>
  <iframe :src="'/pdf/web/viewer.html?file='+pdfUrl"></iframe>
</template>
<script>

export default {
  name: 'Pdf',
  props: {
    pdfUrl: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>
iframe {
  /* width: 960px; */
  width: 1100px;
  max-width: 100%;
  height: 800px;
  margin-left: 50%;
  transform: translateX(-50%);
}
</style>
