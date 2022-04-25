<template>
  <!-- 底部导航 -->
  <div class="docker">
    <!-- BEM block__element--modifier -->
    <div class="docker__item docker__item--active">
      <div class="iconfont">&#xe751;</div>
      <div class="docker__title">首页</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe899;</div>
      <div class="docker__title">购物车</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe626;</div>
      <div class="docker__title">订单</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe8bb;</div>
      <div class="docker__title">我的</div>
    </div>
  </div>
</template>

<style lang="scss">
@import "./style/index.scss";
.docker {
  display: flex;
  position: absolute;
  left: 0;
  width: 100%;
  height: 0.49rem;
  bottom: 0;
  border-top: 0.01rem solid #f1f1f1;
  // background-color: green;
  color: $content-fontcolor;
  &__item {
    flex: 1;
    text-align: center;
    // font-size: 0.2rem;
    // transform: scale(0.5, 0.5);
    // transform-origin: center top;
    .iconfont {
      margin: 0.07rem 0 0.02rem 0;
      font-size: 0.18rem;
    }

    &--active {
      color: $hightlight-color;
    }
  }
  &__title {
    font-size: 0.2rem;
    transform: scale(0.5, 0.5);
    transform-origin: center top;
  }
}
</style>
