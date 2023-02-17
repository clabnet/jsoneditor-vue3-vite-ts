<script setup lang="ts">

import JsonEditor from './components/jsonEditor.vue';

const data = {
  greeting: 'Hello World',
  color: '#ff3e00',
  ok: true,
  values: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15],
}

</script>

<template>
  <div class="app">
    <h1>jsoneditor-vue3-vite-ts</h1>
    <h2>Editor</h2>
    <div class="my-editor">
      <json-editor :source="data" />
    </div>
  </div>
</template>

<style>
.app {
  font-family: sans-serif;
}

.my-editor {
  width: 700px;
  height: 400px;
  display: flex;
}
</style>

