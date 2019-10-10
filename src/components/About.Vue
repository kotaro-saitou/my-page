<template>
  <div class="about">
    <tab-menu></tab-menu>
    <h3>{{ name }}</h3>
    <img class="img" src="../assets/image/me_image.jpg" width="125" />
    <p>Age: 23</p>
    <div class="sns-link">
      <ul>
        <li>
          <a href="https://twitter.com/__kotaro_">Twitter</a>
        </li>
        <li>
          <a href="https://github.com/kotaro-saitou">Github</a>
        </li>
        <li>
          <a href="https://qiita.com/__kotaro_">Qiita</a>
        </li>
      </ul>
    </div>
    <div class="skill">
      <h3>Skill</h3>
      <p>Language</p>
      <ul>
        <li>Ruby</li>
        <li>C#</li>
        <li>Python</li>
      </ul>
      <p>Framework</p>
      <ul>
        <li>Ruby on Rails</li>
        <li>Vue.js</li>
      </ul>
    </div>
  </div>
</template>

<script>
import TabMenu from '@/components/TabMenu'

export default {
  name: 'About',
  components: {
    TabMenu
  },
  data () {
    return {
      name: 'kotaro saito'
    }
  }
}
</script>

<style scoped>
.about {
  text-align: center;
}

.img {
  border-radius: 50%;
}

.sns-link ul {
  list-style-type: none;
  padding-left: 0;
}

.sns-link ul li {
  display: inline;
  padding: 0 5px;
}

.sns-link a {
  display: inline-block;
  background-color: #26a69b;
  color: #fff;
  font-size: 1em;
  line-height: 1;
  text-decoration: none;
  letter-spacing: 0.05em;
  padding: 0.2em 1em;
  border-radius: 3px;
  cursor: pointer;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
  -webkit-tap-highlight-color: transparent;
  transition: 0.3s ease-out;
}

.sns-link a:hover {
  box-shadow: 0 3px 3px 0 rgba(0, 0, 0, 0.14), 0 1px 7px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -1px rgba(0, 0, 0, 0.2);
}

.skill p {
  display: inline-block;
  padding: 0.3em 1em;
  color: #26a69b;
  border: solid 2px #26a69b;
  border-radius: 3px;
  transition: 0.4s;
}

.skill ul {
  list-style-type: none;
  padding-left: 0;
}

.skill ul li {
  display: inline;
  padding: 0 5px;
}
</style>
