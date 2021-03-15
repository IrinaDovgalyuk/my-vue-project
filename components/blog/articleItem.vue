<template>
  <div class="articleItem">
    <a :href="link" class="articleItem__title" target="_blank">{{title}}</a>
    <p class="articleItem__date">{{date}}</p>
    <p class="articleItem__text">{{prew}}</p>
    <p class="articleItem__views">
      Количество просмотров: <span  class="articleItem__views--number">{{views}}</span>
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'NewsArticle',

  props: {
    item: {
      type: Object,
      default: () => ({}),
    },
  },

  computed: {
    title() {
      return this.item.title;
    },
    date() {
      return this.item.date;
    },
    prew() {
      return this.item.prew;
    },
    text() {
      return this.item.text;
    },
    views() {
      return this.item.views;
    },
    link() {
      return this.item.link;
    },
  },
})
</script>

<style scoped>
.articleItem{
  display: flex;
  flex-direction: column;
  justify-items: flex-start;
  align-items: flex-start;
}

.articleItem__title{
  font-size: 24px;
  font-weight: 500;
  margin: 20px;
  color:cadetblue;
  text-decoration: none;
  text-align: left;
}

.articleItem__title:hover {
  text-decoration: underline;
}

.articleItem__date {
  font-size: 16px;
  font-weight: 500;
  margin: 0 20px;
}

.articleItem__text{
  max-width: 500px;
  text-align: justify;
  font-size: 18px;
  font-weight: 300;
  margin: 15px 20px;}

.articleItem__views {
  font-size: 14px;
  font-weight: 500;
  margin: 0 20px 10px;
}

@media only screen and (min-width: 960px) {
  .articleItem__title {
    font-size: 28px;
    margin: 40px 0 10px;
  }

  .articleItem__date {
    margin: 0px;
  }

  .articleItem__text {
    font-size: 20px;
    margin: 10px 0 20px;
  }

  .articleItem__views {
    font-size: 14px;
    font-weight: 500;
    margin: 0 0 10px;
  }
}
</style>
