<template>
<div class="post_container">
  <el-row type="flex" align="center" class="top_title">
    <el-col :offset="2" :span="3">
      标题
    </el-col>
    <el-col :span="19">
      <el-input placeholder="Note your title"></el-input>
    </el-col>
  </el-row>
  <el-row type="flex" align="center" class="top_content">
    <el-col :offset="2" :span="3">
      <img src="~@/assets/header.png" class="header" />
    </el-col>
      <el-col :span="19">
        <el-input type="textarea" :rows="3" placeholder="What's on you mind, Quan?" v-model="textarea">
        </el-input>
      </el-col>
  </el-row>

  <el-row type="flex" align="center" class="top_b">
    <el-col class="top_b_1">
      <img src="~@/assets/icon/5.png" />
      People
    </el-col>
      <el-col>
        <img src="~@/assets/icon/4.png" />
      Check in
    </el-col>
        <el-col>
          <img src="~@/assets/icon/3.png" />
      Mood
    </el-col>
          <el-col>
            <el-button class="top_btn" type="primary">share</el-button>
          </el-col>
  </el-row>

  <div class="status_container">
    <!-- <span>标题</span>
    <el-input placeholder="请输入内容">
      <template slot="prepend">Http://</template>
    </el-input> -->
  </div>
  <div>

  </div>
  <div>

  </div>
</div>
</template>

<script>

</script>

<style>
.post_container {
  background: #FFFFFF;
  box-shadow: 0 2px 6px 0 rgba(47, 83, 151, 0.10);
  border-radius: 6px;
}

.status_container {
  height: 0.6rem;
  line-height: 0.6rem;
}

.top_title {
  height: 0.5rem;
  line-height: 0.5rem;
}

.top_content {
  height: 1rem;
  display: flex;
  align-items: center
}

.top_b {
  height: 0.6rem;
  box-shadow: inset 0 1px 0 0 #F5F7FA;
  display: flex;
  align-items: flex-end;
}

.top_b_1 {
  padding-left: 0.23rem;
}

.top_btn {
  border-radius: 4px;
  width: 1.24rem;
  height: 0.39rem;
  padding: 0 !important;
}

.header {
  width: 0.4rem;
  height: 0.4rem;
  border-radius: 50%
}

/* .status_container span {
  padding-left: 0.46rem;
  width: 0.67rem;
} */
</style>
