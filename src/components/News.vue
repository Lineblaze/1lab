<template>
  <main>
    <h1>Новости</h1>
    <div>
      <div class="article" v-for="(article, index) in news" :key="index">
        <h2><router-link :to='"/article/" + article.id'>{{article.id}} {{article.name}}</router-link></h2>
        <p>{{article.shortDesc}}</p>
      </div>
    </div>
  </main>
</template>

<script>
import news from '../assets/articles.json'

export default {
  name: 'News',
  data(){
      return {
        news
    };
  }
}
</script>

<style scoped>
.article {
  border-bottom: 1px solid #000;
}

.article a {
  text-decoration: none;
  color: green;
}

.article a:hover {
  text-decoration: underline;
}
</style>