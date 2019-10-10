<template>
  <div class="contact">
    <tab-menu></tab-menu>
    <h3>お問い合わせ</h3>
    <p>下記メールアドレスかTwitterにお願いします。</p>
    <div class="link">
      <ul>
        <li>
          <a href="https://twitter.com/__kotaro_">Twitter</a>
        </li>
        <li>
          <p>Email : kotaro.saito27@gmail.com</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import TabMenu from '@/components/TabMenu'

export default {
  name: 'Contact',
  components: {
    TabMenu
  }
}
</script>

<style scoped>

div.contact {
  text-align: center;
}

.link {
  margin-top: 50px;
}

.link ul {
  list-style-type: none;
  padding-left: 0;
}

.link ul li {
  margin-bottom: 30px;
}

.link a {
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

link.a:hover {
  box-shadow: 0 3px 3px 0 rgba(0, 0, 0, 0.14), 0 1px 7px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -1px rgba(0, 0, 0, 0.2);
}

.link p {
  display: inline;
  padding: 0.5em 1em;
  margin: 2em 0;
  color: #232323;
  background: #E6FFE9;
  border-left: solid 10px #26a69b;
  margin: 0;
  padding: 0;
}

</style>
