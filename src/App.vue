<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#apps {
  font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑", Arial, sans-serif;
  width: 100%;
  height: 100%;
}

html {
  width: 100%;
  height: 100%;
  display: table;
}

body {
  margin: 0px;
  padding: 0px;
  display: table-cell;
  height: 100%;
}
</style>
