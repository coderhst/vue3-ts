<template>
  <div class="content">
    <h3 @click="handleDemoClick">Hello</h3>
    <h4 @click="handleClickDemo">name</h4>
    <h4 @click="handleQuickClick"></h4>
    <h5></h5>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: '',
  props: {},
  components: {},
  setup() {
    const name = ref('coderWhy')

    const handleClickDemo = () => {
      console.log('Hello Word')
    }

    const handleDemoClick = () => {
      console.log('12342342')
    }

    const handleQuickClick = () => {
      console.log('Demo Vue')
    }
    return {
      name,
      handleClickDemo,
      handleDemoClick,
      handleQuickClick
    }
  }
})
</script>

<style scoped lang="less"></style>
