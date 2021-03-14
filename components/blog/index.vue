<template>
  <div class="container">
    <div class="mainWrapper">
      <h1 class="title">
        Blog
      </h1>

      <div class="articles">
        <div class="articleItem">
          <h2 class="articleItem__title">Title</h2>
          <p class="articleItem__date">Date</p>
          <p class="articleItem__text">text</p>
          <p class="articleItem__views">Количество просмотров: <span  class="articleItem__views--number">0</span></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'BlogMain',
})
</script>

<style scoped>
.mainWrapper {
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  text-align: center;
}
</style>
