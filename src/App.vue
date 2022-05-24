<template>
  <ColumnList :list="list"></ColumnList>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import ColumnList, { ColumnProps } from './components/ColumnList.vue'
const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'title',
    description: 'jhdjksdhksjdhs',
    avatar: '/logo.png'
  },
  {
    id: 2,
    title: 'title2',
    description: 'jhdjksdhksjdhs',
    avatar: '/logo.png'
  }
]
export default defineComponent({
  name: 'app',
  components: { ColumnList },
  setup () {
    return {
      list: testData
    }
  }
})
</script>
<style>

</style>
