<template>
  <div class="ProjectsItem">
    <a :href="link" class="ProjectsItem__title" target="_blank">{{title}}</a>
    <p class="ProjectsItem__date">{{date}}</p>
    <p class="ProjectsItem__text">{{text}}</p>
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'NewsProject',

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
    text(): any {
      return this.item.text;
    },
    link() {
      return this.item.link;
    },
  },
})
</script>

<style scoped>
.ProjectsItem{
  display: flex;
  flex-direction: column;
  justify-items: flex-start;
  align-items: flex-start;
}

.ProjectsItem__title{
  font-size: 24px;
  font-weight: 500;
  margin: 20px;
  color:#35495e;
  text-decoration: none;
  text-align: left;
}

/*
.ProjectsItem__title:hover {
  text-decoration: underline;
}*/

.ProjectsItem__date {
  font-size: 16px;
  font-weight: 500;
  margin: 0 20px;
}

.ProjectsItem__text{
  max-width: 500px;
  text-align: justify;
  font-size: 18px;
  font-weight: 300;
  margin: 15px 20px;}

.ProjectsItem__views {
  font-size: 14px;
  font-weight: 500;
  margin: 0 20px 10px;
}

@media only screen and (min-width: 960px) {
  .ProjectsItem__title {
    font-size: 28px;
    margin: 40px 0 10px;
  }

  .ProjectsItem__date {
    margin: 0px;
  }

  .ProjectsItem__text {
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
