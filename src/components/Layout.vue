<template>
  <div>
    <el-container>
      <el-aside width="150px">
        <side-bar />
      </el-aside>
      <el-container>
        <el-header>
          <nav-bar />
        </el-header>
        <el-main>
          <main-app />
        </el-main>
        <el-footer>
          <span>Copyright © 2012 大連市XXXX区不動産登録情報ネット
            <br />
            電話番号80004000 営業番号84616600
          </span>

        </el-footer>
      </el-container>
    </el-container>
  </div>

</template>

<script>
import MainApp from './MainApp.vue'
import NavBar from './NavBar.vue'
import SideBar from './SideBar.vue'
export default {
  data () {
    return {}
  },
  components: {
    SideBar,
    MainApp,
    NavBar
  }
}
</script>

<style>
.el-header,
.el-footer {
  background-color: #b8d1b3;
  color: rgb(51, 51, 51);
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #e9eef3;
  color: #333;
  text-align: left;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  /* line-height: 450px; */
  vertical-align: top;
  padding: 5px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
