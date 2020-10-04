<template>
  <div>
    <div id="menu-bg" :class="{ open: hbg }"></div>
    <nav class="nav-head">
      <div class="head-row">
        <div class="head-logo">
          <img src="images/logo_gf.png" alt="ロゴ画像" />
        </div>
        <div class="head-pc-nav">
          <a v-on:mouseover="(company = true), (cnt = 1)" href="#">COMPANY</a>
          <a v-on:mouseover="(products = true), (cnt = 2)" href="#">PRODUCTS</a>
          <a v-on:mouseover="(news = true), (cnt = 3)" href="#">NEWS</a>
          <a v-on:mouseover="(recruit = true), (cnt = 4)" href="#">RECRUIT</a>
          <a class="english" href="#">English</a>
        </div>
        <div id="humberger" class="humberger" v-on:click="hbg = !hbg">
          <div class="bar bar1" :class="{ hbg_btn1: hbg }"></div>
          <div class="bar bar2" :class="{ hbg_btn2: hbg }"></div>
          <div class="bar bar3" :class="{ hbg_btn3: hbg }"></div>
          <div class="hum-menu">MENU</div>
        </div>
      </div>
      <transition>
        <div class="sp-head-hover" v-show="hbg">
          <div class="sp-head-list" id="sp-company">
            <h2>COMPANY　<span>-企業情報-</span></h2>
          </div>
          <div class="sp-head-list" id="sp-products">
            <h2>PRODUCTS　<span>-製作実績-</span></h2>
          </div>
          <div class="sp-head-list" id="sp-news">
            <h2>NEWS　<span>-最新情報-</span></h2>
          </div>
          <div class="sp-head-list" id="sp-recruit">
            <h2>RECRUIT　<span>-採用情報-</span></h2>
          </div>
          <div class="sp-head-mdl">
            <div class="lang-link">japanese / English</div>
            <div class="sp-head-sns">
              <a class="twitter" href="#">
                <i class="fab fa-twitter"></i>
              </a>
              <a class="facebook" href="#">
                <i class="fab fa-facebook-f"></i>
              </a>
            </div>
          </div>
          <div class="head-bottom-link">
            <div class="head-flexbox"><a href="#">サイトマップ</a></div>
            <div class="head-flexbox"><a href="#">サイトポリシー</a></div>
          </div>
          <div class="head-bottom-link">
            <div class="head-flexbox"><a href="#">プライバシーポリシー</a></div>
            <div class="head-flexbox"><a href="#">お問い合わせ</a></div>
          </div>
        </div>
      </transition>

      <transition>
        <div
          v-show="company && cnt == 1"
          class="pc-nav-hover"
          v-on:mouseover="company = true"
          v-on:mouseleave="company = false"
        >
          <h1>COMPANY</h1>
          <span>-企業説明-</span>
          <div class="link-box-pc-head">
            <a href="#">企業情報トップへ</a>
          </div>
          <div class="pc-image-link">
            <div>
              <a href="#"><img src="images/message_pc.jpg" alt="" /></a>
              <p>代表メッセージ</p>
            </div>
            <div class="center">
              <a href="#"><img src="images/about.jpg" alt="" /></a>
              <p>会社概要/アクセス</p>
            </div>
            <div>
              <a href="#"><img src="images/nav_company.jpg" alt="" /></a>
              <p>沿革</p>
            </div>
          </div>
        </div>
      </transition>
      <transition>
        <div
          v-show="products && cnt == 2"
          class="pc-nav-hover"
          v-on:mouseover="products = true"
          v-on:mouseleave="products = false"
        >
          <h1>PRODUCTS</h1>
          <span>-製作実績-</span>
          <div class="link-box-pc-head">
            <a href="#">製作実績トップへ</a>
          </div>
          <div class="pc-image-link pc-image-link-product">
            <div>
              <a href="#"><img src="images/switch.jpg" alt="" /></a>
              <p>家庭用ゲーム</p>
            </div>
            <div>
              <a href="#"><img src="images/iphone.jpg" alt="" /></a>
              <p>ソーシャルゲーム</p>
            </div>
          </div>
        </div>
      </transition>
      <transition>
        <div
          v-show="news && cnt == 3"
          class="pc-nav-hover"
          v-on:mouseover="news = true"
          v-on:mouseleave="news = false"
        >
          <h1>NEWS</h1>
          <span>-最新情報-</span>
          <div class="link-box-pc-head">
            <a href="#">最新情報トップへ</a>
          </div>
          <div class="pc-image-link pc-image-link-product">
            <div>
              <div class="pc-nav-news-txt">
                <a href="#"
                  >2020.10.03　　
                  <span class="tag">コーポレート</span
                  >　　グッドフィールは創立15周年を迎えました</a
                >
              </div>
              <div class="pc-nav-news-txt">
                <a href="#"
                  >2020.10.03　　
                  <span class="tag">リクルート</span
                  >　　　スタッフインタビューを更新しました</a
                >
              </div>
              <div class="pc-nav-news-txt">
                <a href="#"
                  >2020.10.03　　
                  <span class="tag">リクルート</span
                  >　　　サウンドクリエイターの募集を開始しました</a
                >
              </div>
              <div class="pc-nav-news-txt">
                <a href="#"
                  >2020.10.03　　
                  <span class="tag">リクルート</span
                  >　　　新規プロジェクトの立ち上げにつき、中途デザイナーの募集を開始しました</a
                >
              </div>
            </div>
          </div>
        </div>
      </transition>
      <transition>
        <div
          v-show="recruit && cnt == 4"
          class="pc-nav-hover"
          v-on:mouseover="recruit = true"
          v-on:mouseleave="recruit = false"
        >
          <h1>RECRUIT</h1>
          <span>-採用情報-</span>
          <div class="link-box-pc-head">
            <a href="#">採用情報トップへ</a>
          </div>
          <div class="pc-image-link">
            <div>
              <a href="#"><img src="images/message_pc.jpg" alt="" /></a>
              <p>トップメッセージ</p>
            </div>
            <div>
              <a href="#"><img src="images/recruit.jpg" alt="" /></a>
              <p>スタッフインタビュー</p>
            </div>
            <div>
              <a href="#"><img src="images/nav_env.png" alt="" /></a>
              <p>はたらく環境</p>
            </div>
            <div>
              <a href="#"><img src="images/nav_data.png" alt="" /></a>
              <p>データで見るGF</p>
            </div>
          </div>
        </div>
      </transition>
    </nav>
  </div>
</template>
<script>
export default {
  data() {
    return {
      cnt: null,
      company: false,
      products: false,
      news: false,
      recruit: false,
      hbg: false,
    };
  },
};
</script>
<style lang="scss" scoped>
@import "~assets/scss/common.scss";
//ヘッドナビゲーション
#menu-bg {
  position: fixed;
  display: none;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #000;
  opacity: 0.5;
  &.open {
    display: block;
  }
}
.head-logo {
  margin-left: 8px;
  margin-top: 20px;
  width: 120px;
  z-index: 9999;
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
    height: 100%;
    height: 70px;
    top: 20px;
    left: 35px;
    right: 20px;
    border-radius: 30px;
    opacity: 1;
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
    z-index: 9999;
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
  transition: 0.3s;
}
.bar2 {
  top: 24px;
  transition: 0.3s;
}
.bar3 {
  top: 32px;
  transition: 0.3s;
}
.hbg_btn1 {
  transform: translateY(8px) rotate(-45deg);
  transition: 0.3s;
}
.hbg_btn2 {
  transform: translateX(10px);
  opacity: 0;
  transition: 0.3s;
}
.hbg_btn3 {
  transform: translateY(-8px) rotate(45deg);
  transition: 0.3s;
}
.hum-menu {
  position: absolute;
  height: 4px;
  width: 24px;
  top: 40px;
  font-size: 1px;
}

//ホバー時
.sp-head-hover {
  position: fixed;
  top: 60px;
  width: 100%;
  border-top: 1px solid #ddd;
  background-color: #fff;
  font-size: 12px;
  z-index: 9999;

  /* &.open {
    display: block;
  }*/
  @include pc {
    display: none;
  }
}

.sp-head-list {
  height: 70px;
  border-bottom: 1px solid #ddd;
}
.sp-head-list h2 {
  padding-left: 20px;
  font-size: 15px;
  line-height: 70px;
  @include bold;
}
.sp-head-mdl {
  text-align: center;
  margin: 30px 0 30px 0;
}
.lang-link {
  font-size: 15px;
  margin-bottom: 10px;
  @include bold;
}

.sp-head-sns a {
  display: inline-block;
  color: #fff;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  padding-top: 4px;
  line-height: 54px;
}
.sp-head-sns i {
  top: 15px;
  font-size: 24px;
}
.twitter {
  background-color: $twitter;
  margin-right: 15px;
}
.facebook {
  background-color: $facebook;
}
.head-bottom-link {
  display: flex;
  text-align: center;
  height: 60px;
}
.head-flexbox {
  width: 50%;
  line-height: 60px;
  border: 1px solid #c4c4c4;
  border-bottom: none;
  border-left: none;
}
.pc-nav-hover {
  background-color: #fff;
  position: relative;
  top: -30px;
  text-align: center;
  transition: 0.3s;
  padding-bottom: 30px;
  border-radius: 0 0 30px 30px;
}
.pc-nav-hover h1 {
  font-size: $font-B;
  padding-top: 80px;
  @include bold;
}
.pc-image-link {
  margin-top: 40px;
  display: flex;
  justify-content: center;
}
.pc-image-link img {
  width: 270px;
  height: 170px;
  border-radius: 30px;
}
.pc-image-link div {
  margin-right: 10px;
  margin-left: 10px;
}
/*.center {
  margin: 0 20px;
}*/
.link-box-pc-head {
  text-align: center;
  margin-top: 20px;
}
.link-box-pc-head a {
  font-size: 14px;
  @include bold;
  @include link-box(15px, 40px, 30px);
}
.v-enter {
  opacity: 0;
  transform: translateY(-18px);
}
.v-enter-to {
  opacity: 1;
}
.v-leave {
  transform: translateY(18px);
  opacity: 1;
}
.v-leave-to {
  display: none;
}
.v-enter-active {
  transition: all 500ms;
}
.v-leave-active {
  transition: all 100ms;
}
.pc-nav-news-txt {
  text-align: left;
  border-bottom: 1px solid #ddd;
  padding-top: 10px;
  padding-bottom: 10px;
  font-size: 14px;
  @include bold;
}
.tag {
  color: #fff;
  font-size: 12px;
  padding: 2px 20px;
  background: #c0c0c0;
  border-radius: 30px;
  @include bold;
}
</style>