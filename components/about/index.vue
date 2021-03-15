<template>
  <div class="container">
    <div class="mainWrapper">
      <h1 class="title">
        About me
      </h1>

      <div class="about">
        <div class="aboutAuthor">
          <img src="https://placeimg.com/400/400/nature" alt="" class="aboutAuthor__img">
          <div class="aboutAuthor__name">Ирина Д</div>
          <div class="aboutAuthor__text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dicta, molestiae omnis! Porro neque veniam facere optio provident animi quidem facilis reiciendis nam fugit, dolorem labore ab hic velit nobis officiis iusto voluptatum possimus omnis vel atque eos doloribus. Eos explicabo ad perferendis adipisci facere veritatis tenetur nostrum odit dolorum iure?</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'About',
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

.aboutAuthor__img {
  height: 200px;
  width: 200px;
  border-radius: 50%;
  border: cadetblue solid 5px;
}

.aboutAuthor__name {
  font-size: 24px;
  font-weight: 500;
  margin: 20px;
  color:#35495e;
}

.aboutAuthor__text {
  max-width: 500px;
  text-align: justify;
  font-size: 18px;
  font-weight: 300;
  margin: 15px;
}

@media only screen and (min-width: 960px) {
  .aboutAuthor__name {
    font-size: 28px;
    margin: 40px;
  }

  .aboutAuthor__text {
    font-size: 20px;
    margin: 20px;
  }
}
</style>
