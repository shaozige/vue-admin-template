<template>
  <el-tabs v-model="activeName" type="card" @tab-click="handleClick">
    <el-tab-pane label="待办" name="todo">待办</el-tab-pane>
    <el-tab-pane label="日程" name="schedule">日程</el-tab-pane>
    <el-tab-pane label="已办" name="done">已办</el-tab-pane> 
  </el-tabs>
</template>
<script>
  export default {
    data() {
      return {
        activeName: 'todo'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    }
  };
</script>