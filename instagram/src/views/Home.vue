<template>
  <div class="home">
    <ul>
      <article-list
        v-for="article in articles"
        :key="article.id"
        :article="article"
      ></article-list>
    </ul>
  </div>
</template>

<script>
import ArticleList from '@/components/ArticleList'

export default {
  name: 'Home',
  components: {
    ArticleList,
  }
}
</script>
