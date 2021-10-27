<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import {Notification} from '@arco-design/web-vue';
import '@arco-design/web-vue/es/notification/style/css';
const hello = ()=>{
Notification.info('sdd')
}
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
<button @click="hello">12</button>
  <button>123</button>

</template>

<style>

</style>
