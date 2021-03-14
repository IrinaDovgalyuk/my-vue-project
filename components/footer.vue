<template>
  <div class="social">
    <a href="https://www.facebook.com/" target="_blank">Facebook </a>
    <a href="https://www.instagram.com/" target="_blank">instagram</a>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Footer',
})
</script>

<style scoped>
.social{
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
