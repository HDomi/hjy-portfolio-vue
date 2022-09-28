<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import MainTitle from './components/MainTitle.vue'
import SubTitle from './components/SubTitle.vue'
</script>

<template>
  <header>
    <img alt="My Photo" class="logo" src="@/assets/my_photo.jpg" width="170"/>
    <div class="wrapper">
      <MainTitle maintit="황재영의 Portfolio입니다." />
      <SubTitle subtit="안녕하세요." />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/myself">Myself</RouterLink>
        <RouterLink to="/portfolio">Dev_</RouterLink>
        <RouterLink to="/design">Design</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
        <RouterLink to="/finish">Finish</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 15px;
}

nav {
  width: 100%;
  font-size: 1.1rem;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--active-text);
  font-weight: bold;
  background-color: hsla(160, 100%, 37%, 1);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  margin: 10px 5px 0 5px;
  display: inline-block;
  padding: 0 1rem;
  border-radius: 10px;
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
  }

  nav {
    text-align: left;
    margin-left: -0.4rem;
    font-size: 1.1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
