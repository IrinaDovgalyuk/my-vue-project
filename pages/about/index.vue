<template>
  <div>
    <About />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({})
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 700;
  font-size: 28px;
  color: #35495e;
  letter-spacing: 1px;
  margin: 30px 0;
}
@media only screen and (min-width: 960px) {
  .title {
     font-size: 48px;
     margin: 50px 0;
  }
}
</style>
