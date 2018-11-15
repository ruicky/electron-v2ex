<template>
<div class=".favourite_container">
  <el-row class="r_header">
    <el-col class="r_headerText" :span="20">
      分类
    </el-col>
    <el-col :span="4">
      <img src="~@/assets/icon/1.png" alt="electron-vue" />
    </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/2.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/7.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/8.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/9.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/10.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
  <el-row class="r_header">
    <el-col :span="20">
      <img class="r_header_left_img" src="~@/assets/icon/6.png" alt="electron-vue" />
      最热
    </el-col>
      <el-col :span="4" class="r_header_right_text">
        15
      </el-col>
  </el-row>
</div>
</template>

<script>

</script>

<style>
.favourite_container {
  background: #FFFFFF;
  box-shadow: 0 2px 6px 0 rgba(232, 239, 253, 0.1);
  border-radius: 6px;
}
.post_container{
    height: 2.39rem;
}
.r_header {
  height: 0.67rem;
  line-height: 0.67rem;
  font-size: 13px;
  color: #202841;

}

.r_headerText {
  padding-left: 0.32rem;

}

.r_header:first-child {
  color: #919BAB;
  font-size: 0.19rem;
  box-shadow: inset 0 -1px 0 0 #F5F7FA;
}

.r_header_left_img {
  width: 16px;
  height: 16px;
  padding-left: 0.38rem;
  padding-right: 0.24rem;
}

.r_header_right_text {
  font-size: 0.13rem;
  color: #919EAB;
}
</style>
