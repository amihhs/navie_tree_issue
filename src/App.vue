<script setup>
import {NTree} from 'naive-ui'
import {ref} from 'vue'
const options = ref([{
          label: 'l-0',
          key: 'v-0',
          depth: 1,
          isLeaf: false
        }])
async function loadHandle(node) {
  console.log('loadHandle')
    return false
}
</script>

<template>
  <div>
    <n-tree :data="options"  @load="loadHandle"></n-tree>
  </div>
</template>

<style scoped>

</style>
