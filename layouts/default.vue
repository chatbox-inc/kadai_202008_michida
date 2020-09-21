<template>
  <div class="default-area">
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
    <hr />
    <Nuxt />
    <footer>
      <div class="foot-wrap">
        <nav class="foot-pc-nav">
          <div class="container-fluid">
            <div class="footer-pc-row">
              <div class="pc-nav-el">
                <h2>
                  <a href="#">COMPANY</a>
                </h2>
                <ul class="pc-nav-ul">
                  <li>
                    <a href="#">代表メッセージ</a>
                  </li>
                  <li>
                    <a href="#">会社概要/アクセス</a>
                  </li>
                  <li>
                    <a href="#">沿革</a>
                  </li>
                </ul>
              </div>
              <div class="pc-nav-el">
                <h2>
                  <a href="#">PRODUCTS</a>
                </h2>
                <ul class="pc-nav-ul">
                  <li>
                    <a href="#">家庭用ゲーム</a>
                  </li>
                  <li>
                    <a href="#">ソーシャルゲーム</a>
                  </li>
                </ul>
              </div>
              <div class="pc-nav-el">
                <h2>
                  <a href="#">NEWS</a>
                </h2>
                <ul class="pc-nav-ul">
                  <li>
                    <a href="#">コーポレートニュース</a>
                  </li>
                  <li>
                    <a href="#">リクルートニュース</a>
                  </li>
                  <li>
                    <a href="#">ゲームニュース</a>
                  </li>
                </ul>
              </div>
              <div class="pc-nav-el">
                <h2>
                  <a href="#">RECRUIT</a>
                </h2>
                <ul class="pc-nav-ul">
                  <li>
                    <a href="#">新卒採用</a>
                  </li>
                  <li>
                    <a href="#">キャリア採用</a>
                  </li>
                  <li>
                    <a href="#">スタッフインタビュー</a>
                  </li>
                  <li>
                    <a href="#">はたらく環境</a>
                  </li>
                  <li>
                    <a href="#">データで見るGF</a>
                  </li>
                  <li>
                    <a href="#">採用ニュース</a>
                  </li>
                  <li>
                    <a href="#">FAQ</a>
                  </li>
                </ul>
              </div>
              <div class="pc-nav-el">
                <ul>
                  <li>
                    <a class="pc-nav-sns pc-nav-twitter" href="#">
                      <i class="fab fa-twitter pc-sns"></i>Twitter
                    </a>
                  </li>
                  <li>
                    <a class="pc-nav-sns pc-nav-facebook" href="#">
                      <i class="fab fa-facebook-square pc-sns"></i>Facebook
                    </a>
                  </li>
                </ul>
              </div>
            </div>
            <div class="pc-nav-bottom-row">^</div>
          </div>
        </nav>
        <aside class="sp-aside">
          <a class="twitter" href="#">
            <i class="fab fa-twitter"></i>
          </a>
          <a class="facebook" href="#">
            <i class="fab fa-facebook-f"></i>
          </a>
        </aside>
        <nav class="bottom-nav-sp">
          <div class="bottom-nav-sp-row">
            <div class="sp-bottom-row">
              <div class="bottom-link">
                <a href="#">サイトマップ</a>
              </div>
              <div class="bottom-link">
                <a href="#">サイトポリシー</a>
              </div>
            </div>
            <div class="sp-bottom-row">
              <div class="bottom-link">
                <a href="#">プライバシーポリシー</a>
              </div>
              <div class="bottom-link">
                <a href="#">お問い合わせ</a>
              </div>
            </div>
            <div class="copy-write">© Good-Feel Co., Ltd.</div>
          </div>
        </nav>
      </div>
      <nav class="bottom-nav-pc">
        <div class="bottom-nav-pc-row">
          <div class="pc-bottom-left">
            <div class="bottom-link">
              <a href="#">サイトマップ</a>
            </div>
            <div class="bottom-link">
              <a href="#">サイトポリシー</a>
            </div>
            <div class="bottom-link">
              <a href="#">プライバシーポリシー</a>
            </div>
            <div class="bottom-link">
              <a href="#">お問い合わせ</a>
            </div>
          </div>
          <div class="pc-bottom-right">© Good-Feel Co., Ltd.</div>
        </div>
      </nav>
      <!-- ここまでbottom-nav-pc -->
    </footer>
  </div>
</template>

<style lang="scss">
@import "~assets/scss/common.scss";

img {
  width: 100%;
}

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

//ここからfooter
footer {
  background-color: rgba(221, 221, 221, 0.4);
}
.foot-wrap {
  max-width: 1200px;
  margin: 0 auto;
}
.foot-pc-nav {
  display: none;
  @include pc {
    display: block;
    margin-bottom: 20px;
  }
}
.footer-pc-row {
  display: flex;
  padding-top: 70px;
}
.pc-nav-el {
  margin-right: 30px;
  width: 200px;
}
.pc-nav-el h2 {
  font-size: 26px;
  margin-bottom: 10px;
  padding-bottom: 20px;
  border-bottom: solid 1px #b8b8b8;
}
.pc-nav-ul li {
  font-size: 12px;
  font-weight: bold;
  padding-top: 10px;
  padding-bottom: 10px;
}
.pc-nav-sns {
  color: #fff;
  font-size: 30px;
  border-radius: 30px;
  display: block;
  margin: 0 auto;
  width: 300px;
  height: 65px;
  padding-top: 10px;
  text-align: center;
  margin-bottom: 10px;
}
.pc-sns {
  margin-right: 10px;
}
.pc-nav-twitter {
  background: #1da1f2;
}
.pc-nav-facebook {
  background: #4267b2;
}
.pc-nav-bottom-row {
  width: 100%;
  background: #ffb32e;
  color: #fff;
  font-size: 45px;
  height: 60px;
  border-radius: 30px;
  text-align: center;
  cursor: pointer;
}
.sp-aside {
  display: block;
  width: 200px;
  padding-top: 70px;
  padding-bottom: 30px;
  margin: 0 auto;
  text-align: center;
  @include pc {
    display: none;
  }
}
.sp-aside a {
  position: relative;
  display: inline-block;
  color: #fff;
  width: 50px;
  height: 50px;
  padding: 10px;
  border-radius: 50%;
  line-height: 54px;
}
.sp-aside i {
  position: absolute;
  top: 15px;
  font-size: 24px;
}
.fa-twitter {
  right: 12px;
}
.fa-facebook-f {
  right: 15px;
}
.twitter {
  background-color: #1da1f2;
  margin-right: 15px;
}
.facebook {
  background-color: #4267b2;
}
.bottom-nav-sp {
  display: block;
  @include pc {
    display: none;
  }
}
.bottom-nav-sp-row {
  display: flex;
  flex-direction: column;
  width: 280px;
  margin: 0 auto;
}
.sp-bottom-row {
  display: flex;
  justify-content: center;
}
.bottom-link {
  font-size: 14px;
  font-weight: bold;
  margin-right: 10px;
  margin-bottom: 30px;
  display: inline-block;
}
.bottom-nav-pc-row {
  display: none;
  @include pc {
    padding-left: 60px;
    padding-right: 60px;
    border-top: solid 1px #b8b8b8;
    padding-top: 20px;
    display: flex;
    justify-content: space-between;
  }
}
.bottom-nav-pc-row {
  .bottom-link {
    font-size: 12px;
  }
}
.copy-write {
  text-align: center;
}
</style>
