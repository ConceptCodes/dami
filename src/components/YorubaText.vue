<template>
  <div class="yoruba-text">
   <textarea v-model="yoText" placeholder="Enter Yoruba Translation Here." required></textarea>
   <div>
</template>

<script>
export default {
  name: 'YorubaText',
  props: {
    yoText: String
  }
}
</script>
<style scoped>

</style>
