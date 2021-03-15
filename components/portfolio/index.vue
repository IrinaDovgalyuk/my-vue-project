<template>
  <div class="mainWrapper">
    <h1 class="title">
      Портфолио
    </h1>

    <div class="ProjectsList">
      <NewsProject
        v-for="ProjectItem of listProjects"
        :key="ProjectItem.id"
        :item="ProjectItem"
      />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import NewsProject from './pojectItem.vue';

const listProjects = [
  {
    title: 'ДЗ к двадцать четвертому занятию',
    date: '14.03.2021',
    text: 'Прочитайте теоретическую часть по Layouts в nuxt, и добавьте свой собственный layout в проект созданный на занятии, а также свою страницу по адресу test/mypage.',
    link: 'https://github.com/IrinaDovgalyuk/ons-e-commerce',
  },
  {
    title: 'Проект модуля HTML&& CSS',
    date: '07.03.2021',
    text: 'Выбрать любой из имеющихся макетов и создать сайт.',
    link: 'https://github.com/IrinaDovgalyuk/ozon-homework/tree/main/project-html-css',
  },
  {
    title: 'ДЗ к тринадцатому занятию',
    date: '29.11.2020',
    text: 'Напишите функцию, переворачивающую переданную строчку ( word —> drow ). Напишите реализацию алгоритма ROT-13 https://ru.wikipedia.org/wiki/ROT13 только для английского алфавита.',
    link: 'https://irinadovgalyuk.github.io/js-ozon/homework-13/',
  },
  {
    title: 'ДЗ к одиннадцатому занятию',
    date: '29.11.2020',
    text: 'Напишите функцию, которая будет проверять длину переданного в качестве аргумента слова. В случае если слово меньше 10 символов, функция должна выводить в консоль сообщение о том что слово подходит, если больше либо равно 10 символам - сообщение о том что слово слишком длинное',
    link: 'https://irinadovgalyuk.github.io/js-ozon/homework-11/',
  },
  {
    title: 'Д/З ко второму занятию',
    date: '29.11.2020',
    text: 'Создайте репозиторий на Github. В проекте, который вы зальете, должны быть карточки товаров с Ozon или с любого другого  интернет-магазина. При клике на карточки можно переходить на эти товары на внешнем источнике.',
    link: 'https://irinadovgalyuk.github.io/',
  },
];

export default Vue.extend({
  name: 'Potfolio',

  components: {
    NewsProject,
  },

  data() {
    return {
      listProjects,
    };
  },
})
</script>

<style scoped>
.mainWrapper {
  max-width: 500px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  text-align: center;
}
</style>
