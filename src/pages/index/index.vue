<template>
  <div>
    <!-- 顶部 -->
    <div class="header">
      <div class="left">老伴</div>
      <div class="right">
        <a href="#">电影</a>
        <a href="#">图书</a>
        <a href="#">广播</a>
        <a href="#">小组</a>
        <!-- 小程序自带的标签 图标 -->
        <icon type="search" color="#05b512"/>
      </div>
    </div>
    <!-- 热映区域 -->
    <div class="section">
      <div class="top">
        <div class="title">影院热映</div>
        <a href="#">更多</a>
      </div>
      <!-- 横向滚动区域 -->
       <scroll-view
        scroll-x
        scroll-with-animation
        >
          <div class="item">1</div>
          <div class="item">2</div>
          <div class="item">3</div>
          <div class="item">4</div>
          <div class="item">5</div>
          <div class="item">6</div>
        
      </scroll-view>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
// 豆绿
$douGreen: #05b512;
.header {
  height: 105rpx;
  display: flex;
  align-items: center;
  padding: 0 40rpx;
  justify-content: space-between;
  border-bottom: 2rpx solid $douGreen;
  .left {
    color: $douGreen;
    font-size: 50rpx;
    font-weight: 700;
  }
  .right {
    display: flex;
    a {
      font-size: 30rpx;
      margin-right: 30rpx;
      &:nth-child(1) {
        color: #2585e8;
      }
      &:nth-child(2) {
        color: #a5806a;
      }
      &:nth-child(3) {
        color: #e4ab1d;
      }
      &:nth-child(4) {
        color: #30b9cd;
      }
    }
    icon {
      color: $douGreen;
    }
  }
}
// 区域
.section{
  .top{
    display: flex;
    padding: 25rpx 30rpx 0;
    justify-content: space-between;
    .title{
      font-size:34rpx;
      font-weight: 500;
    }
    a{
      font-size:28rpx;
      color:$douGreen;
    }
  }
  // 滚动区域
  scroll-view{
    width: 100%;
    overflow: hidden;
    white-space: nowrap;
    .item{
      width: 200rpx;
      height: 250rpx;
      background-color: $douGreen;
      margin-right: 10rpx;
      display: inline-block;
    }
  }

}
</style>
