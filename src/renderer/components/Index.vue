<template>
<div class="container">
  <el-container>
    <el-aside>
      <Favourite />
    </el-aside>
    <el-container>
      <el-header>
        <PostPage />
      </el-header>
      <el-main>
        <ContentPage />
      </el-main>
    </el-container>
  </el-container>
</div>
</template>

<script>
import Favourite from './Favourite';
import PostPage from './PostPage';
import ContentPage from './ContentPage';

export default {
  name: 'landing-page',
  components: {
    Favourite,
    PostPage,
    ContentPage,
  },
  methods: {
    open(link) {
      this.$electron.shell.openExternal(link);
    },
  },
};
</script>

<style>
.container {
  font-size: 0.16rem;
  font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;
}

.el-header{
  height: 2.39rem !important;
}

</style>
