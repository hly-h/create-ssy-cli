<script setup lang="ts">
// eslint-disable-next-line @typescript-eslint/no-unused-vars
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="container">
    <div class="pic">
      <a href="https://vitejs.dev" target="_blank">
      <img src="./assets/vite.svg" class="logo" alt="Vite logo" width="130" height="130"/>
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo" alt="Vue logo" width="130" height="130"/>
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/ssy.svg" class="logo" alt="SSY logo" width="130" height="130"/>
    </a>
    </div>
    <div class="wrapper">
      <HelloWorld msg="Vite + Vue3 + SSYUI" style="margin-left: 240px;"/>
      <div style="margin-bottom: 20px;">
        <SButton>SButton</SButton>
        <SLink color="green">测试Link组件</SLink>
      </div>
    </div>
  <p></p>
  <RouterView />
</div>
</template>

<style scoped>
.container{
  text-align: center;
  width: 900px;
  margin-left: 160px;
}

.pic{
  display: flex;
  justify-content: center; /* 可根据需要设置图标在水平方向的对齐方式 */
  gap: 20px; /* 调整图像之间的间距 */
  margin-bottom: 50px;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    margin-left: 10px;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
