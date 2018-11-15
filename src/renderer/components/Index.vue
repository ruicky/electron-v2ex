<template>
<div class="container">
  <el-container>
    <el-aside width="30%">
      <Favourite />
    </el-aside>
    <el-container>
      <el-header>
        Header
      </el-header>
      <el-main>Main</el-main>
    </el-container>
  </el-container>
</div>
</template>

<script>
import Favourite from './Favourite';
export default {
  name: 'landing-page',
  components: {
    Favourite,
  },
  methods: {
    open(link) {
      this.$electron.shell.openExternal(link);
    },
  },
};
</script>

<style>
.el-header{
  background-color: #B3C0D1;
  color: #333;
  text-align: center;
}


.el-main {
  background-color: #E9EEF3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

.container {
  font-size: 0.16rem;
}
</style>
