<template>
  <div class="container-fluid">
    <div class="slider">
      <div class="slide-list">
        <a href="#">
          <img src="/images/img_list1.png" alt="MONKEY BARRELS" />
        </a>
      </div>
    </div>
    <hr />
    <div id="products" class="products">
      <div class="products-wrap">
        <div class="products-title">
          <h1>PRODUCTS</h1>
          <p>-制作実績-</p>
        </div>
        <div class="row products-slide">
          <div class="col-4 product-image">
            <a href="#">
              <img src="/images/img_slide.png" alt />
              <p>毛糸のカービィ</p>
            </a>
          </div>
          <div class="col-4 product-image">
            <a href="#">
              <img src="/images/img_slide1.png" alt />
              <p>ヨッシークラフトワールド</p>
            </a>
          </div>
          <div class="col-4 product-image">
            <a href="#">
              <img src="/images/img_slide2.png" alt />
              <p>ワリオランドシェイク</p>
            </a>
          </div>
        </div>
        <div class="link-box">
          <a href="#">制作実績一覧</a>
        </div>
      </div>
    </div>
    <hr />
    <div id="news" class="news">
      <div class="news-wrap">
        <div class="news-title">
          <h1>NEWS</h1>
          <p>-ニュース-</p>
        </div>
        <div class="news-container">
          <div class="row">
            <article class="test news-box col-12 col-md-4">
              <div class="article-content">
                <div class="article-img">
                  <img src="/images/designer.jpg" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <span>リクルート</span>
                  <span>2020.08.26</span>
                </div>
                <div class="article-txt">
                  <p>【大阪事業所】新規プロジェクト立ち上げにつき、中途デザイナーの募集を開始しました</p>
                </div>
              </div>
            </article>
            <article class="test news-box col-12 col-md-4">
              <div class="article-content">
                <div class="article-img">
                  <img src="/images/onlineSeminar.png" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <span>リクルート</span>
                  <span>2020.07.13</span>
                </div>
                <div class="article-txt">
                  <p>オンライン会社説明会について</p>
                </div>
              </div>
            </article>
            <article class="test news-box col-12 col-md-4">
              <div class="ariticle-content">
                <div class="article-img">
                  <img src="/images/data.png" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <span>リクルート</span>
                  <span>2020.03.09</span>
                </div>
                <div class="article-txt">
                  <p>グッド・フィールを大解剖「データでみるGF」公開！</p>
                </div>
              </div>
            </article>
          </div>
          <div class="link-box">
            <a href="#">ニュース一覧へ</a>
          </div>
        </div>
      </div>
    </div>
    <hr />
    <div id="recruit" class="recruit">
      <div class="recruit-wrap">
        <div class="recruit-container">
          <div class="row recruit-top">
            <div class="test col-12 recruit-title-area">
              <div class="recruit-txt-area">
                <h1>RECRUIT</h1>
                <p>世の中をカラフルに</p>
              </div>
            </div>
          </div>
          <div class="row recruit-bottom">
            <div class="test col-4 company-area">
              <div class="recruit-txt-area">
                <h2>COMPANY</h2>
                <p>-企業情報-</p>
              </div>
            </div>
            <div class="test col-4 message-area">
              <div class="recruit-txt-area">
                <h2>MESSAGE</h2>
                <p>-代表メッセージ-</p>
              </div>
            </div>
            <div class="test col-4 about-area">
              <div class="recruit-txt-area">
                <h2>ABOUT</h2>
                <p>-会社概要-</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~assets/scss/common.scss";

.container-fluid {
  /* 作業用css */
  .test {
    border: 1px solid #ddd;
  }
  max-width: 100%;
  //トップスライド
  .slider {
    .slide-list {
      @include sp {
        height: 200px;
        img {
          height: 200px;
        }
      }
      img {
        width: 100%;
      }
    }
  }

  //productsエリア
  .products {
    @include sp {
      height: 520px;
    }
    .products-wrap {
      .products-title {
        text-align: center;
      }
      .products-slide {
        .product-image {
        }
      }
      .link-box {
        text-align: right;
        @include sp {
          text-align: center;
        }
      }
    }
  }

  //newsエリア
  .news {
    .news-wrap {
      padding: 40px 0 60px;
      .news-title {
        text-align: center;
      }
    }
    .news-container {
      margin: 40px 0;
      .news-box {
        @include sp {
          height: 300px;
          margin-bottom: 20px;
        }
      }
      .link-box {
        text-align: right;
        @include sp {
          text-align: center;
        }
      }
    }
  }

  //recruitエリア
  .recruit {
    .recruit-wrap {
      .recruit-container {
        .recruit-txt-area {
          text-align: center;
        }
        .recruit-top {
          @include sp {
            height: 220px;
          }
          .recruit-title-area {
            background-image: url("/images/recruit.jpg");
          }
        }
        .recruit-bottom {
          @include sp {
            height: 150px;
          }
          .company-area {
            background-image: url("/images/company.jpg");
          }
          .message-area {
            background-image: url("/images/message.jpg");
          }
          .about-area {
            background-image: url("/images/about.jpg");
          }
        }
      }
    }
  }
}
</style>
