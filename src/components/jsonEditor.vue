<script setup lang="ts">
  import JsonEditorVue from 'json-editor-vue'

  interface Props {
    source: any
  }

  const props = defineProps<Props>()
</script>

<template>
  <div class="ml-5 w-100% h-98%">
    <n-card hoverable :bordered="true" class="shadow-sm rounded-xl ml-5">
      <div class="border-green-300 border-solid border-0 overflow-y-scroll h-175">
        <json-editor-vue v-model="props.source" :readOnly="true" />
      </div>
    </n-card>
  </div>
</template>
