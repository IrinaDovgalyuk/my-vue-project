<template>
  <div class="header">
    <div>
      <div class="links">
        <a href="/about" class="button--green">
          About
        </a>
        <a href="/blog" class="button--grey">
          Blog
        </a>
        <a href="/" class="button--green">
          Home
        </a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Header',
})
</script>

<style scoped>
.header {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  text-align: center;
}

.links {
  padding-top: 15px;
}
</style>
