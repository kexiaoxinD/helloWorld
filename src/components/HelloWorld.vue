<template>
  <div>
    <el-container>
      <el-header>
        <div class="header-logo">
          <img src="@/assets/logo.png">
        </div>
        <div class="header-title">小新Demo系统</div>
        <div class="header-menu">
          <!-- <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
            <el-menu-item index="1">处理中心</el-menu-item>
            <el-submenu index="2">
              <template slot="title">我的工作台</template>
              <el-menu-item index="2-1">选项1</el-menu-item>
              <el-menu-item index="2-2">选项2</el-menu-item>
              <el-menu-item index="2-3">选项3</el-menu-item>
              <el-submenu index="2-4">
                <template slot="title">选项4</template>
                <el-menu-item index="2-4-1">选项1</el-menu-item>
                <el-menu-item index="2-4-2">选项2</el-menu-item>
                <el-menu-item index="2-4-3">选项3</el-menu-item>
              </el-submenu>
            </el-submenu>
            <el-menu-item index="3" disabled>消息中心</el-menu-item>
            <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>
          </el-menu> -->
        </div>
        <div class="header-person">
          <el-dropdown>
            <span class="el-dropdown-link">
              科小新<i class="el-icon-arrow-down el-icon--right"></i>
            </span>
            <el-dropdown-menu slot="dropdown">
              <el-dropdown-item>个人中心</el-dropdown-item>
              <el-dropdown-item>退出系统</el-dropdown-item>
            </el-dropdown-menu>
          </el-dropdown>
        </div>
      </el-header>
      <el-container>
        <el-aside width="200px">
          <el-menu
            default-active="2"
            class="el-menu-vertical-demo"
            background-color="#353535"
            text-color="#fff"
            active-text-color="#ffd04b">
            <el-submenu index="1">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>导航一</span>
              </template>
              <el-menu-item-group>
                <template slot="title">分组一</template>
                <el-menu-item index="1-1">选项1</el-menu-item>
                <el-menu-item index="1-2">选项2</el-menu-item>
              </el-menu-item-group>
              <el-menu-item-group title="分组2">
                <el-menu-item index="1-3">选项3</el-menu-item>
              </el-menu-item-group>
              <el-submenu index="1-4">
                <template slot="title">选项4</template>
                <el-menu-item index="1-4-1">选项1</el-menu-item>
              </el-submenu>
            </el-submenu>
            <el-menu-item index="2">
              <i class="el-icon-menu"></i>
              <span slot="title">导航二</span>
            </el-menu-item>
            <el-menu-item index="3" disabled>
              <i class="el-icon-document"></i>
              <span slot="title">导航三</span>
            </el-menu-item>
            <el-menu-item index="4">
              <i class="el-icon-setting"></i>
              <span slot="title">导航四</span>
            </el-menu-item>
          </el-menu>
        </el-aside>
        <el-container>
          <el-main>Main</el-main>
          <el-footer>版权所有 ©2018 小新工作室</el-footer>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data () {
      return {
        msg: this.testPropweties //'Welcome to Your Vue.js App   TEST 科小新'
      }
    }
  }
</script>

  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .el-header {
    background-color: #ececec ;
    padding: 0;
    position: fixed;
    top: 0px;
    left: 0px;
    z-index: 1;
    width: 100%;
    color: #353535;
    line-height: 70px;
    padding-left: 30px;
    padding-right: 30px;
    height: 70px !important;
    border-bottom: 1px solid #eceef0;
  }

  .header-logo {
    float: left;
    height: 70px;
    line-height: 70px;
  }

  .header-logo img {
    height: 50px;
    vertical-align: middle;
  }

  .header-menu {
    float: left;
  }

  .header-title {
    float: left;
    padding-left: 10px;
    font-weight: bold;
    font-size: 20px;
    letter-spacing: 3px;
    text-shadow: 0.1em 0.1em 0.2em #777676;
  }
  .header-person {
    float: right;
  }

  .el-aside {
    overflow-x: hidden;
    overflow-y: auto;
    transition: width .28s;
    position: fixed;
    top: 70px;
    bottom: 0;
    left: 0;
    width: 200px;
    color: #c5c5c5;
    background-color: #353535;
  }
  
  .el-main {
    background-color: #fff;
    color: #333;
    text-align: center;
    line-height: 460px;
  }

  .el-footer {
    background-color: #EEE;
    line-height: 40px;
    height: 40px !important;
    text-align: center;
    font-size: 12px;
    vertical-align: middle;
    color: #666;
  }
</style>
