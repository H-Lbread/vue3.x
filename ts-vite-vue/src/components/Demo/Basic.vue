<script setup lang="ts">
import { ref } from 'vue'
// import css from "../assets/index.css";

defineProps({
  msg: String
})

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
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
<!--    Demo  count ++
  <template>
      <div>默认的count：{{ state.count }}</div>
      <button @click="increment">增加</button>
  </template>

  <script setup lang="ts">
      import { reactive,computed } from "vue";
      type DState = {
          count:number,
          double:number
      }
      const state: DState = reactive({
          count: 0,
          double:computed(()=>state.count * 2)
      })
      function increment(){
          state.count++
      }
  </script>
-->

