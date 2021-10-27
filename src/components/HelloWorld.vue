<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})
import {Trigger} from '@arco-design/web-vue';
// import '@arco-design/web-vue/es/trigger/style/css';
const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <p>
    Recommended IDE setup:
    <a href="https://code.visualstudio.com/" target="_blank">VSCode</a>
    +
    <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
  </p>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button type="button" @click="count++">count is: {{ count }}</button>
  <p>
<Trigger :render-to-body="false" trigger="click" show-arrow class="demo-basic" position="top">
      <span>Hover Me</span>
      <template #content>
        123
        <input type="button" value="12">
      </template>
    </Trigger> to test hot module replacement.
  </p>
  
</template>

<style>
a {
  color: #42b983;
}
.demo-basic {
  padding: 10px;
  width: 200px;
  background-color: var(--color-bg-popup);
  border-radius: 4px;
  box-shadow: 0 2px 8px 0 rgba(0, 0, 0, 0.15);
}
</style>
