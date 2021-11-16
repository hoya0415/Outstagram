<template>
  <li class="article-box">
    <div class="article-box-bar">
      <div class="article-box-bar-content">
        <div class="canvas">
          <img :src="require('@/assets/proImg' + article.id + '.jpg')">
        </div>
        <p class="nickname">{{ article.nickname }}</p>
        <div class="option-dots">
          <b-icon icon="three-dots"></b-icon>
        </div>
      </div>
    </div>
    <div class="image">
      <!-- <img :src="require('../assets/img' + article.id + '.jpg')"> -->
      <img :src="article.img_url">
    </div>
    <div class="article-content">
      <div class="icons">
        <b-icon icon="heart" scale="1.5"></b-icon>
        <b-icon icon="chat" scale="1.5"></b-icon>
        <img class="icon" :src="require('@/assets/paper_plane_icon.png')">
        <b-icon icon="bookmark" scale="1.5"></b-icon>
      </div>
      <div>
        <p class="article-content-boldtext">좋아요 {{article.like_cnt}}개</p>
      </div>
      <div>
        <span class="article-content-boldtext">{{ article.nickname }} </span> 
        <span class="article-content-text">{{ article.content }} </span>
      </div>
      <div class="article-content-comment">
        댓글 21개 모두 보기
      </div>
      <div class="created">
        {{ article.created }} 전
      </div>
    </div>

  </li>
</template>

<script>
export default {
  name: 'ArticleListItem',
  props:{
    article: Object,
  },
  data: function () {
    return {
    }
  },

}
</script>

<style>
  .article-box {
    max-height: inherit;
    margin-bottom: 15px;
    border: 0 solid #000;
    list-style: none;
    display: flex;
    flex-direction: column;
    margin: 2px 0 30px 0;
  }
  .article-box-bar {
    border: 1px solid rgb(218, 218, 218); 
    width: 100%;
    height: 69px;
  }
  .article-box-bar-content {
    position: relative;
    max-width: 100%;
    padding: 23px 4px 14px 16px;
    
  }
  .canvas {
    background-image: url("../assets/ring.png");
    width: 42px;
    height: 42px;
    position: absolute;
    top: 13px;
    left: 17px;
  }
  .canvas img {
    border-radius: 50%;
    width: 34px;
    height: 34px;
    text-align: right;
    position: absolute;
    top: 4.5px;
    left: 4px;
  }
  
  .nickname {
    font-weight: bold;
    vertical-align: middle;
    display: inline;
    text-align: start;
    position: absolute;
    margin: 0;
    left: 70px;
  }
  .option-dots {
    display: inline;
    position: absolute;
    right: 20px;
  }
  .image {
    display: block;
    width: 100%;
  }
  .image img {
    width: 100%;
    overflow-y: hidden;
  }
  img {
    margin: 0;
    padding: 0;
    border: 0;
    font: inherit;
    vertical-align: baseline;
  }
  .article-content {
    min-width: 335px;
    padding: 0 16px;
    width: 100%;
    min-width: 80px;
    display: flex;
    flex-direction: column;
    text-align: start;
  }
  .article-content-boldtext {
    font-weight: bold;
    font-size: 14px;
  }
  .article-content-text {
    font-size: 14px;
    overflow: hidden;
    white-space: nowrap;
    text-overflow: ellipsis;
    display: block;
  }
  .article-content-comment {
    font-size: 14px;
    color: #8E8E8E;
    margin: 10px 0;
  }
  .created {
    font-size: 10px;
    color: #8E8E8E;
  }
  .icons > * {
    margin: 13px 15px;
  }
  .icon {
    width: 24px;
    margin: 8px;
    display: inline-block;
    overflow: visible;
    vertical-align: -0.15em;
    }
</style>