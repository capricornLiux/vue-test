<template>
  <div id="app">
    <column-list :list="data"></column-list>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import 'bootstrap/dist/css/bootstrap.min.css'
import ColumnList, { ColumnProps } from './components/ColumnList.vue'

const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'xxx',
    description: 'sdf'
    // avatar: 'sdfs'
  },
  {
    id: 1,
    title: 'xxx',
    description: 'sdf',
    avatar: 'sdfs'
  },
  {
    id: 1,
    title: 'xxx',
    description: 'sdf',
    avatar: 'sdfs'
  },
  {
    id: 1,
    title: 'xxx',
    description: 'sdf',
    avatar: 'sdfs'
  }
]
export default defineComponent({
  name: 'App',
  components: {
    ColumnList
  },
  setup () {
    return {
      data: testData
    }
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
