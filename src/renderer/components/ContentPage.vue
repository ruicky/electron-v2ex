<template>
<div class="content_container">
  <!-- 头像部分 -->
  <div class="top_container">
    <div>
      <img class="avatar" src="~@/assets/header.png" />
      </div>
      <div class="top_text">
        <span>ruicky</span>
        <span>6 hours ago</span>
      </div>
    </div>
    <!-- 内容部分 -->
    <div class="main_container">
      <p>
        Ocean breeze, salty air, sun kissed hair. That endless summer take me there.
      </p>
      <img src="~@/assets/Bitmap.png" />
    </div>
      <!-- 评论部分 -->
      <div class="discuss_container">
        <img class="avatar" src="~@/assets/header.png" />
        <div class="discuss_content">
          <p>极简生活是风靡全球的一种最有价值的生活方式！一项正在全世界范围内推行的运动！</p>
          <p>极简生活不是苦行僧式的自虐，而是一种更为人性化的、经济的、环保的、轻松愉悦的生活方式。</p>
          <p>极简生活的美好，不是它会带走什么，而是它会给予什么。</p>
          <p>极简生活是《知乎日报》、《人民日报》、《搜狐时尚》、《今日中国》、中共中央宣传部委托新华通讯社主办《半月谈》、金羊网、大河网、《检查日报》等各大媒体发文力推的最有价值的生活方式。</p>
          <p>现代最有影响力的极简运动倡导者之一乔舒亚·贝克尔（JoshuaBecker）告诉你，怎样实施极简主义生活，以及它为什么是一种最有价值的生活方式！</p>
          <p>极简生活是扎克伯格、乔布斯、爱因斯坦等都致力践行的生活方式，他们都是极简生活的信徒。</p>
        </div>
      </div>
    </div>
</template>

<style>
.content_container {
  background: #FFFFFF;
  box-shadow: 0 2px 6px 0 rgba(47, 83, 151, 0.10);
  border-radius: 4px;
  padding-left: 0.3rem;
  padding-right: 0.23rem;
  padding-bottom: 0.28rem;

}

.top_container {
  padding-top: 0.23rem;
  display: flex;
}

.top_text {
  display: flex;
  flex-direction: column;
  padding-left: 0.12rem;
}

.top_text span:nth-child(2) {
  padding-top: 0.04rem;
  font-size: 0.10rem;
  color: #919EAB;
  text-align: left;
}

.avatar {
  width: 0.4rem;
  height: 0.4rem;
  border-radius: 50%;
}

.main_container img {
  display: block;
  width: 100%;

}

.discuss_container {
  display: flex;
  padding-top: 0.25rem;
  align-items: center;
}

.discuss_content {
  margin-left: 0.16rem;
  border: 1px solid #EDF1F6;
  border-radius: 0.2rem;
  font-size: 0.12rem;
  width: 100%;
}
</style>
