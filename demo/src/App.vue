<script setup lang="ts">
// demo/src/App.vue
import { Button, Input, SimpleShowInput } from "@openx-rc/ui";

import HelloWorld from "./components/HelloWorld.vue";

import { ref } from "vue";

const simpleShowInput = ref("你好");
</script>

<template>
  <section>
    <div>
      <a href="https://vitejs.dev" target="_blank">
        <img src="/vite.svg" class="logo" alt="Vite logo" />
      </a>
      <a href="https://vuejs.org/" target="_blank">
        <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
      </a>
    </div>
    <HelloWorld msg="Vite + Vue" />

    <Button>1111</Button>
    <Input />

    <SimpleShowInput v-model="simpleShowInput" />
  </section>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
