<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <div
    style="
      height: 100vh;
      background-image: url('https://thumb.tildacdn.com/tild3130-6234-4739-b461-323535666534/-/format/webp/photo_2022-03-23_14-.jpg');
      width: 100%;
      background-size: cover;
      -webkit-background-size: cover;
      -moz-background-size: cover;
      -o-background-size: cover;
      background-repeat: no-repeat;
      background-position: center center;
      position: absolute;
      background-attachment: fixed;
      top: 0;
      left: 0;
      transform: translate3d(0, 0, 0);
      -webkit-transform: translate3d(0, 0, 0);
      -moz-transform: unset;
    "
  ></div>
  <header>
    <div class="wrapper">
      <HelloWorld msg="Коворкинг в центре Сочи" />
    </div>
  </header>

  <!-- <RouterView /> -->
</template>

<style>
@import "@/assets/base.css";

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
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
  body {
    display: flex;
    place-items: center;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr;
    padding: 0 2rem;
  }

  header {
    display: grid;
    grid-template-columns: 1fr;
    padding: 0 2rem;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  .logo {
    margin: 0 2rem 0 0;
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
