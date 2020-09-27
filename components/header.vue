<template>
  <div>
    <nav class="nav-head">
      <div class="head-row">
        <div class="head-logo">
          <img src="images/logo_gf.png" alt="ロゴ画像" />
        </div>
        <div class="head-pc-nav">
          <a href="#">COMPANY</a>
          <a href="#">PRODUCTS</a>
          <a href="#">NEWS</a>
          <a href="#">RECRUIT</a>
          <a class="english" href="#">English</a>
        </div>
        <div id="humberger" class="humberger">
          <div class="bar bar1"></div>
          <div class="bar bar2"></div>
          <div class="bar bar3"></div>
          <div class="hum-menu">MENU</div>
        </div>
      </div>
    </nav>
  </div>
</template>
<style lang="scss" scoped>
@import "~assets/scss/common.scss";
//ヘッドナビゲーション
.head-logo {
  margin-left: 8px;
  margin-top: 20px;
  width: 120px;
  @include pc {
    margin-left: 30px;
    width: 150px;
  }
}
.nav-head {
  z-index: 10;
  width: 100%;
  background-color: #fff;
  position: fixed;
  top: 0;
  height: 60px;
  @include pc {
    width: 95%;
    position: fixed;
    height: 70px;
    top: 20px;
    left: 35px;
    right: 20px;
    border-radius: 30px;
    opacity: 0.9;
  }
}
.head-row {
  display: flex;
  justify-content: space-between;
}

.head-pc-nav {
  display: none;
  @include pc {
    display: block;
    line-height: 70px;
  }
}
.head-pc-nav a {
  font-size: 14px;
  font-weight: bold;
  margin-right: 30px;
  margin-left: 40px;
}
.english {
  color: #fff;
  padding-right: 0px;
  padding: 5px 10px 5px 10px;
  background: #ffb32e;
  border-radius: 30px;
}
//humbergerメニューエリア
.humberger {
  display: block;
  position: fixed;
  top: 2px;
  right: 10px;
  height: 24px;
  width: 30px;
  @include pc {
    display: none;
  }
}

.bar {
  position: absolute;
  height: 3px;
  width: 30px;
  background-color: #000;
  border-radius: 2px;
  display: inline-block;
}
.bar1 {
  top: 16px;
}
.bar2 {
  top: 24px;
}
.bar3 {
  top: 32px;
}
.hum-menu {
  position: absolute;
  height: 4px;
  width: 24px;
  top: 40px;
  font-size: 1px;
}
</style>