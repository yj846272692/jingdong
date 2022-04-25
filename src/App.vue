<template>
  <!-- 顶部导航 -->
  <div class="wrapper">
    <!-- 定位 -->
    <div class="wrapper__position">
      <span class="iconfont">&#xe8ba;</span>
      江苏省南京市栖霞区羊山北路1号
      <span class="iconfont position__notice">&#xe60d;</span>
    </div>

    <!-- 搜索区域 -->
    <div class="wrapper__search">
      <span class="iconfont">&#xe632;</span>
      <span class="search__test">山姆会员商店优惠商品</span>
    </div>

    <!-- banner -->
    <div class="wrapper__banner">
      <img
        src="https://soft2176-use.oss-cn-hangzhou.aliyuncs.com/banner/jingdong/banner1.jpg"
        class="wrapper__banner__img"
        alt=""
      />
    </div>
    <!-- <div>123</div> -->

    <!-- icon宫格区 -->
    <div class="icons">
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E8%B6%85%E5%B8%82.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">超市便利</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E5%8C%BB%E8%8D%AF%E5%81%A5%E5%BA%B7.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">医药健康</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E5%A4%A7%E7%89%8C%E5%85%8D%E8%BF%90.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">大牌免运</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E5%AE%B6%E5%B1%85.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">家居</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E6%B0%B4%E6%9E%9C%E5%BA%97.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">水果店</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E7%AD%BE%E5%88%B0.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">签到</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E7%BA%A2%E5%8C%85.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">红包</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E8%8F%9C%E5%B8%82%E5%9C%BA.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">菜市场</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E8%9B%8B%E7%B3%95.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">蛋糕</p>
      </div>
      <div class="icons__item">
        <img
          src="https://soft2176-yj.oss-cn-hangzhou.aliyuncs.com/JingDong/%E9%B2%9C%E8%8A%B1.png"
          class="icons__item__img"
        />
        <p class="icons__item__desc">鲜花</p>
      </div>
    </div>

    <!-- gap 分割条 -->
    <div class="gap"></div>
  </div>

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
.wrapper {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0.5rem;
  padding: 0 0.18rem;
  &__position {
    position: relative;
    padding: 0.16rem 0.16rem 0.16rem 0;
    font-size: 0.16rem;
    @include ellipse;
    .iconfont {
      font-size: 0.2rem;
    }
    // background: green;
    .position__notice {
      position: absolute;
      right: 0;
    }
    color: $content-fontcolor;
  }
  &__search {
    margin-bottom: 0.12rem;
    line-height: 0.32rem;
    border-radius: 0.16rem;
    background-color: $background-color;
    color: $placeholder-color;
    .iconfont {
      display: inline-block;
      padding: 0 0.12rem 0 0.16rem;
      font-style: 0.2rem;
    }
    &__text {
      // display: inline-block;
      font-size: 0.14rem;
    }
  }
  &__banner {
    height: 0;
    overflow: hidden;
    // hack技巧，预留高度防抖（图片高/图片宽）
    padding-bottom: 25.4%;
    &__img {
      width: 100%;
    }
  }
}
.icons {
  display: flex;
  flex-wrap: wrap;
  margin-top: 0.16rem;
  &__item {
    width: 20%;
    &__img {
      display: block;
      width: 0.4rem;
      height: 0.4rem;
      margin: 0 auto;
    }
    &__desc {
      margin: 0.06rem 0.06rem 0.06rem 0;
      text-align: center;
      color: $content-fontcolor;
    }
  }
}

.gap {
  margin: 0 -0.18rem;
  height: 0.1rem;
  background-color: #f1f1f1;
}
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
