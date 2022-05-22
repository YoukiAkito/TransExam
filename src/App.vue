<template>

<el-row class="row-bg" justify="center">
  <el-card  class="maincard">
    
      <topic></topic>
      
  </el-card>
</el-row>

</template>

<script setup>
import topic from './components/topic.vue'
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

.maincard {
  max-width:600px;
}
</style>