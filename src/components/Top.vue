<template>
  <div id="top">
    <tab-menu></tab-menu>
    <div id="main" class="has-text-centered">
      <h1 class="title is-1">Welcome to My Portfolio</h1>
      <!-- a href="https://bulma.io" target="_blank">
        <img
          src="https://bulma.io/images/made-with-bulma.png"
          alt="Made with Bulma"
          width="128"
          height="24"
        />
      </a>-->
    </div>
    <vue-particles
      color="#dedede"
      :particleOpacity="0.7"
      :particlesNumber="80"
      shapeType="circle"
      :particleSize="4"
      linesColor="#dedede"
      :linesWidth="1"
      :lineLinked="true"
      :lineOpacity="0.4"
      :linesDistance="150"
      :moveSpeed="3"
      :hoverEffect="true"
      hoverMode="grab"
      :clickEffect="true"
      clickMode="push"
    ></vue-particles>
  </div>
</template>

<script>
import TabMenu from '@/components/TabMenu'

export default {
  name: 'Top',
  components: {
    TabMenu
  }
}
</script>

<style>

html, body, #app {
  height: 100%;
}

#top {
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
  width: 100vw;
  position: relative;
  left: 50%;
  right: 50%;
  margin-left: -50vw;
  margin-right: -50vw;
}

#main {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateY(-50%) translateX(-50%);
}

h1 {
  color: #000033 !important;
  font-family: "Dosis", sans-serif;
}
</style>
