<template>
  <div>
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
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "~assets/scss/common.scss";
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
  background: $twitter;
}
.pc-nav-facebook {
  background: $facebook;
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
  background-color: $twitter;
  margin-right: 15px;
}
.facebook {
  background-color: $facebook;
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