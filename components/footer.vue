<template>
  <div class="footer">
    <div class="social">
      <a href="https://www.facebook.com/" target="_blank" class="socialIcon">Facebook </a> •
      <a href="https://www.instagram.com/" target="_blank" class="socialIcon">Instagram</a>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Footer',
})
</script>

<style scoped>
.footer {
  padding-top: 20px;
}
.social{
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.socialIcon{
  text-decoration: none;
  font-size: 16px;
  font-weight: 400;
  margin: 0 15px;
  color: cadetblue;
}

@media only screen and (min-width: 960px) {
  .footer {
    padding: 20px 0;
  }
  .social{
    flex-direction: row;
  }
  .socialIcon{
    font-size: 16px;
    font-weight: 400;
    margin: 0 30px;
  }
}
</style>
