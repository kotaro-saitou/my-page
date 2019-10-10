<template>
  <div class="work">
    <tab-menu></tab-menu>
    <h3>Portfolio</h3>
    <div class='work-box'>
      <a href="https://engineer-link.herokuapp.com"><h2>Engineer Link</h2></a>
      <p class="content">Engineer Linkは、エンジニアとエンジニアが気軽にメッセージを送りあえるサービスです。</p>
      <p class="skill">Ruby on Rails, Heroku, Rspec, AmazonS3</p>
    </div>
    <div class='work-box'>
      <a href="https://kotaro-saitou.github.io/my-page"><h2>My portfolio</h2></a>
      <p class="content">Vue.jsを勉強してみたくて思いつきで勉強して作ったポートフォリオサイトです。勉強始めて３日で作ったので改善の余地だらけ。</p>
      <p class="skill">Vue.js</p>
    </div>
  </div>
</template>

<script>
import TabMenu from '@/components/TabMenu'

export default {
  name: 'Work',
  components: {
    TabMenu
  }
}
</script>

<style scoped>

div.work {
  text-align: center;
}

.work-box {
  width: 80%;
  margin: 0 auto;
  margin-top: 30px;
  padding: 0.5em 1em;
  color: #5d627b;
  background: white;
  border-top: solid 5px #5d627b;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.22);
}

</style>
