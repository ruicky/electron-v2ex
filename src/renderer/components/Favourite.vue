<template>
<div class="favourite_container">
  <el-row class="r_header r_header_first">
    <el-col class="r_headerText" :span="20">
      分类
    </el-col>
    <el-col :span="4">
      <img src="~@/assets/icon/1.png" alt="electron-vue" />
    </el-col>
  </el-row>
  <div v-for="item in noteData" @click="handleChange(item.id)">
    <el-row class="r_header" :class="{r_header_active:item.id == activeId}" >
      <el-col :span="20">
        <img   class="r_header_left_img" :src="item.icon" alt="electron-vue" />
        {{item.name}}
      </el-col>
      <el-col :span="4" class="r_header_right_text" :class="{r_header_right_text_active:item.id == activeId}">
        {{item.number}}
      </el-col>
    </el-row>

  </div>
  <!-- <el-row class="r_header">
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
  </el-row> -->
</div>
</template>

<script>
const noteData = [{
  name: '最热',
  id: 'hot',
  icon: require('../assets/icon/2.png'),
  number: 2,
},
{
  name: '全部',
  id: 'all',
  icon: require('../assets/icon/6.png'),
  number: 10,
},
{
  name: '技术',
  id: 'tech',
  icon: require('../assets/icon/7.png'),
  number: 1,
},
{
  name: '创意',
  id: 'creative',
  icon: require('../assets/icon/8.png'),
  number: '30+',
},
{
  name: '好玩',
  id: 'play',
  icon: require('../assets/icon/9.png'),
  number: '',
},
{
  name: 'Apple',
  id: 'apple',
  icon: require('../assets/icon/10.png'),
  number: '',
},
];
export default {
  data() {
    return {
      noteData,
      activeId: '',
    };
  },
  name: 'landing-page',
  methods: {
    open(link) {
      this.$electron.shell.openExternal(link);
    },
    handleChange(id) {
      this.activeId = id;
    },
  },
};
</script>

<style>
.favourite_container {
  background: #FFFFFF;
  box-shadow: 0 2px 6px 0 rgba(232, 239, 253, 0.1);
  border-radius: 6px;
}

.post_container {
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

.r_header_first {
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

/* 选中样式 */

.r_header_active {
  background: #1F8EFA;
  box-shadow: 0 24px 48px 0 rgba(49, 127, 203, 0.20);
  border-radius: 6px;
  font-size: 0.156rem;
  color: #FFFFFF;
  text-align: left;
}

.r_header_right_text_active {
  font-size: 0.13rem;
  color: #FFFFFF;
}
</style>
