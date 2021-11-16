<template>
  <div class="home">
    <ul>
      <article-list-item
        v-for="article in articles"
        :key="article.id"
        :article="article"
        :imgUrl="article.img_url"
        :profileImgUrl="article.profile_img"
      ></article-list-item>
    </ul>
  </div>
</template>

<script>
import ArticleListItem from '@/components/ArticleListItem'

export default {
  name: 'Home',
  components: {
    ArticleListItem,
  },
  data: function(){
    return {
      articles: [
        {
          id: 1,
          nickname: 'bibber_',
          profile_img: 'https://scontent-ssn1-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/s640x640/255312829_463411148727922_3981182849482448762_n.webp.jpg?_nc_ht=scontent-ssn1-1.cdninstagram.com&_nc_cat=110&_nc_ohc=nnrG5XtPKA0AX85Eu8p&edm=AP_V10EBAAAA&ccb=7-4&oh=11e009e88ae39d55c87073e11946e5f9&oe=6198C4EA&_nc_sid=4f375e%20640w',
          content: '우리집 드릴의 고롱소리였다',
          tags: '#고양이 #그림 #만화 #인스타툰 #일상툰 #주먹꾹 #웹툰' ,
          // img_url: 'https://scontent-ssn1-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/s640x640/256405259_382712540220086_6279090665353943615_n.webp.jpg?_nc_ht=scontent-ssn1-1.cdninstagram.com&_nc_cat=102&_nc_ohc=3sVLlW7OyqgAX81JCk_&edm=AABBvjUBAAAA&ccb=7-4&oh=54e7b56a4a838c656c98e5186700bec4&oe=6198C9BD&_nc_sid=83d603',
          img_url: 'https://picsum.photos/600/300/?image=1',
          like_cnt: '1,183',
          created: '4시간'
        },
        {
          id: 2,
          nickname: 'luv._.bbangsil',
          profile_img: 'https://scontent-ssn1-1.cdninstagram.com/v/t51.2885-19/s150x150/176143532_469483087641407_1566983376298369391_n.jpg?_nc_ht=scontent-ssn1-1.cdninstagram.com&_nc_cat=1&_nc_ohc=NOd9oCncvjAAX9fuBPV&edm=AEF8tYYBAAAA&ccb=7-4&oh=3a23b731b270e65669b462af7a509615&oe=6199F7BE&_nc_sid=a9513d',
          content: '빵시리 이쁜짓!!!!🤎 엄마는 맨날 이쁜짓 시키더라🙄 제나랑 마요랑 개이투 했다구여ㅎㅎ 즐거워따😆',
          tags: '#므에르시앙' ,
          img_url: 'https://scontent-ssn1-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/s640x640/257463567_319343076321658_6270103621061356371_n.jpg?_nc_ht=scontent-ssn1-1.cdninstagram.com&_nc_cat=110&_nc_ohc=s0rMps8qakcAX8wX4UC&edm=APU89FABAAAA&ccb=7-4&oh=ffd454e882d2bf58725df764e386d3e7&oe=6199D8E9&_nc_sid=86f79a',
          like_cnt: '3,357',
          created: '5시간'
        },
      ],
    }
  }
}
</script>

<style scoped>
.home {
  margin-top: 54px;
  display: flex;
  flex-direction: column;
  width: 100%;
  align-items: stretch;
}
ul {
  padding-left: 0;
}
</style>
