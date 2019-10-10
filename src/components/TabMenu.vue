<template>
  <div>
    <ul class='nav'>
      <li v-for="(item, index) in items" :key=index>
        <router-link v-bind:to=item.path>
          {{ item.title }}
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'TabMenu',
  data () {
    return {
      items: [
        {title: 'Home', path: '/'},
        {title: 'About', path: '/about'},
        {title: 'Works', path: '/work'},
        {title: 'Contact', path: '/contact'}
      ]
    }
  }
}
</script>

<style scoped>
.nav {
  display: flex;
  justify-content: center;
  margin-bottom: 50px;
}
.nav > li + li {
  margin-left: 24px;
}
ul {
  padding: 0;
  list-style: none;
}
.nav a {
  text-decoration: none;
  color: black;
}
a.router-link-exact-active {
  font-weight: bold;
}
</style>
