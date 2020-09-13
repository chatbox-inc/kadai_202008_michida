<template>
  <div class="default-area">
    <nav class="nav-head">
      <div class="container">
        <div class="row">
          <div class="col-md-4 col-5">
            <img src="images/logo_gf.png" alt="ロゴ画像" />
          </div>
          <div class="col-md-8 pc-nav">
            <a href="#">COMPANY</a>
            <a href="#">PRODUCTS</a>
            <a href="#">NEWS</a>
            <a href="#">RECRUIT</a>
            <a href="#">English</a>
          </div>
          <div id="humberger" class="humberger">
            <div class="bar bar1"></div>
            <div class="bar bar2"></div>
            <div class="bar bar3"></div>
            <div class="hum-menu">MENU</div>
          </div>
        </div>
      </div>
    </nav>
    <hr />
    <Nuxt />
    <footer>
      <nav class="pc-nav">
        <div class="container-fluid">
          <div class="row">
            <div class="col-md-2">
              <h2>
                <a href="#">COMPANY</a>
              </h2>
              <ul>
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
            <div class="col-md-2">
              <h2>
                <a href="#">PRODUCTS</a>
              </h2>
              <ul>
                <li>
                  <a href="#">家庭用ゲーム</a>
                </li>
                <li>
                  <a href="#">ソーシャルゲーム</a>
                </li>
              </ul>
            </div>
            <div class="col-md-2">
              <h2>
                <a href="#">NEWS</a>
              </h2>
              <ul>
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
            <div class="col-md-2">
              <h2>
                <a href="#">RECRUIT</a>
              </h2>
              <ul>
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
            <div class="col-md-4">
              <ul>
                <li>
                  <a href="#">twitter</a>
                </li>
                <li>
                  <a href="#">facebook</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="row">
            <button>^</button>
          </div>
        </div>
      </nav>
      <aside class="sp-aside">
        <i class="fab fa-twitter"></i>
        <i class="fab fa-facebook-f"></i>
      </aside>
      <nav class="bottom-nav">
        <div class="container">
          <div class="row bottom-row">
            <div class="bottom-link col-6 col-lg-2">
              <a href="#">サイトマップ</a>
            </div>
            <div class="bottom-link col-6 col-lg-2">
              <a href="#">サイトポリシー</a>
            </div>
            <div class="bottom-link col-6 col-lg-2">
              <a href="#">プライバシーポリシー</a>
            </div>
            <div class="bottom-link col-6 col-lg-2">
              <a href="#">お問い合わせ</a>
            </div>
            <div class="copy-write">© Good-Feel Co., Ltd.</div>
          </div>
        </div>
      </nav>
    </footer>
  </div>
</template>

<style lang="scss">
@import "~assets/scss/common.scss";
.default-area {
  img {
    width: 100%;
  }
  //ヘッドナビゲーション
  .nav-head {
    @include sp {
      height: 60px;
      .pc-nav {
        display: none;
      }
    }
  }
  //hambergerメニューエリア
  .humberger {
    position: fixed;
    top: 2px;
    right: 0;
    display: none;
    height: 24px;
    width: 24px;
    @include sp {
      display: inline-block;
    }
    .bar {
      position: absolute;
      left: 0;
      height: 4px;
      width: 24px;
      background-color: #000;
      border-radius: 2px;
      display: inline-block;
    }
    .bar1 {
      top: 0;
    }
    .bar2 {
      top: 10px;
    }
    .bar3 {
      top: 20px;
    }
    .hum-menu {
      font-size: 4px;
      top: 30px;
    }
  }
  //footerエリア
  footer {
    .pc-nav {
      @include sp {
        display: none;
      }
      .container-fluid {
        padding: 0;
      }
    }

    .sp-aside {
      display: none;
      @include sp {
        display: block;
        width: 200px;
        margin: 0 auto;
        text-align: center;
      }
    }
    //一番下メニュー
    .bottom-nav {
      .bottom-row {
        @include sp {
          width: 340px;
          margin: 0 auto;
          .copy-write {
            text-align: center;
          }
        }
      }
    }
  }
}
</style>
