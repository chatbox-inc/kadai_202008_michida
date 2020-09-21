<template>
  <div class="top-page">
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
        <div class="products-slide">
          <div class="product-image">
            <a href="#">
              <img src="/images/img_slide.png" alt />
              <p>毛糸のカービィ</p>
            </a>
          </div>
          <div class="product-image">
            <a href="#">
              <img src="/images/img_slide1.png" alt />
              <p>ヨッシークラフトワールド</p>
            </a>
          </div>
          <div class="product-image">
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
    <!-- ここまでproductsエリア -->
    <div id="news" class="news">
      <div class="news-wrap">
        <div class="news-title">
          <h1>NEWS</h1>
          <p>-ニュース-</p>
        </div>
        <div class="news-container">
          <div class="news-row">
            <article class="news-box">
              <div class="article-content">
                <div class="article-img">
                  <img src="/images/designer.jpg" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <div class="tag">
                    <span class="r-tag">リクルート</span>
                    <span class="new">NEW!</span>
                  </div>
                  <div class="date">2020.08.26</div>
                </div>
                <div class="article-txt">
                  <p>【大阪事業所】新規プロジェクト立ち上げにつき、中途デザイナーの募集を開始しました</p>
                </div>
              </div>
            </article>
            <article class="news-box">
              <div class="article-content">
                <div class="article-img">
                  <img src="/images/onlineSeminar.png" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <div class="tag">
                    <span class="r-tag">リクルート</span>
                    <span class="new">NEW!</span>
                  </div>
                  <div class="date">2020.07.13</div>
                </div>
                <div class="article-txt">
                  <p>オンライン会社説明会について</p>
                </div>
              </div>
            </article>
            <article class="news-box">
              <div class="article-content">
                <div class="article-img">
                  <img src="/images/data.png" alt="リクルート" />
                </div>
                <div class="article-tag">
                  <div class="tag">
                    <span class="r-tag">リクルート</span>
                  </div>
                  <div class="date">2020.03.09</div>
                </div>
                <div class="article-txt">
                  <p>グッド・フィールを大解剖「データでみるGF」公開！</p>
                </div>
              </div>
            </article>
          </div>
          <!-- news-row -->
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
          <div class="recruit-top">
            <div class="recruit-title-area recruit-flex">
              <div class="recruit-txt-area recruit-top-txt">
                <h1>RECRUIT</h1>
                <p>世の中をカラフルに</p>
              </div>
            </div>
          </div>
          <div class="recruit-bottom">
            <div class="company-area recruit-flex">
              <div class="recruit-txt-area">
                <h2>COMPANY</h2>
                <p>-企業情報-</p>
              </div>
            </div>
            <div class="message-area recruit-flex">
              <div class="recruit-txt-area">
                <h2>MESSAGE</h2>
                <p>-代表メッセージ-</p>
              </div>
            </div>
            <div class="about-area recruit-flex">
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
.top-page {
  max-width: 100%;
}

//作業用
.test {
  border: 1px solid #ddd;
}
//トップスライド
.slider {
  margin-top: 60px;
  height: 205px;
  background-size: cover;
  background-image: url("/images/img_list1.png");
  @include pc {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 0;
    height: 760px;
    background-image: url("/images/company.jpg");
  }
}
.slide-list {
  display: none;
  @include pc {
    display: block;
    height: 510px;
    width: 1037px;
    margin: auto;
  }
}
.slide-list img {
  height: 100%;
  border-radius: 30px;
}
//productsエリア
.products {
  //height: 520px;
  height: 100%;
}
.products-wrap {
  padding: 40px 0 60px;
}
.products-title {
  text-align: center;
}
.products-title h1 {
  font-size: 20px;
  margin: 0;
  font-weight: bold;
}
.products-slide {
  display: flex;
}
.link-box {
  text-align: center;
  @include pc {
    text-align: right;
  }
}
//newsエリア
.news {
  background-color: rgba(221, 221, 221, 0.4);
}
.news-wrap {
  padding: 40px 0 30px;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}
.news-box {
  width: 95%;
  margin: 10px auto;
  margin-bottom: 20px;
  background-color: #fff;
  border-radius: 30px;
  @include pc {
    width: 32%;
    max-width: 390px;
    height: 380px;
    margin: 0 auto;
    margin-right: 2%;
  }
}
.article-content {
  width: 90%;
  margin: 20px auto;
}
.article-tag {
  display: flex;
  justify-content: space-between;
}
.article-tag .tag {
  color: #fff;
  margin-top: 8px;
  margin-bottom: 8px;
  font-size: 6px;
}
.r-tag {
  padding: 2px 30px;
  background: #c0c0c0;
  border-radius: 30px;
}
.new {
  color: red;
  font-weight: bold;
}
.article-tag .date {
  margin-top: 8px;
  margin-bottom: 8px;
  text-align: right;
  font-size: 12px;
  font-weight: bold;
  @include pc {
    font-size: 14px;
  }
}
.article-txt {
  font-size: 12px;
  font-weight: bold;
  @include pc {
    font-size: 16px;
  }
}
.news-title {
  text-align: center;
}
.news-title h1 {
  margin: 0;
  font-size: 20px;
  font-weight: bold;
  @include pc {
    font-size: 30px;
  }
}
.news-container {
  margin: 40px 0;
}
.news-row {
  display: flex;
  flex-direction: column;
  @include pc {
    flex-direction: row;
  }
}
.article-img img {
  border-radius: 30px;
}
.link-box {
  text-align: center;
  margin-top: 20px;
  margin-bottom: 30px;
  @include pc {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    text-align: right;
    margin-top: 30px;
  }
}
.link-box a {
  color: #fff;
  background-color: #ffb32e;
  padding: 18px 60px;
  border-radius: 30px;
}

//recruitエリア
.recruit-container {
  display: flex;
  flex-direction: column;
}
.recruit-txt-area {
  padding-top: 20px;
  text-align: center;
  width: 90%;
  height: 70%;
  margin: 0 auto;
  background-color: #fff;
  border-radius: 30px;
  opacity: 0.8;
  @include pc {
    padding-top: 60px;
  }
}
.recruit-top-txt {
  padding-top: 30px;
  @include pc {
    padding-top: 100px;
  }
}
.recruit-txt-area h2 {
  font-size: 22px;
  font-weight: bold;
  @include pc {
    font-size: 35px;
  }
}
.recruit-txt-area p {
  font-size: 14px;
  font-weight: bold;
}
.recruit-flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.recruit-top {
  height: 250px;
  background-image: url("/images/recruit.jpg");
  background-size: cover;
  @include pc {
    height: 580px;
  }
}
.recruit-title-area {
  height: 250px;
  font-weight: bold;
  @include pc {
    height: 600px;
  }
}
.recruit-title-area h1 {
  font-size: 30px;
  font-weight: bold;
  @include pc {
    font-size: 45px;
  }
}
.recruit-title-area p {
  font-size: 18px;
  @include pc {
    font-size: 24px;
  }
}
.recruit-bottom {
  display: flex;
  height: 150px;
  @include pc {
    height: 300px;
  }
}

.company-area {
  flex: 1;
  background-image: url("/images/company.jpg");
  background-size: cover;
}
.message-area {
  flex: 1;
  background-image: url("/images/message.jpg");
  background-size: cover;
}
.about-area {
  flex: 1;
  background-image: url("/images/about.jpg");
  background-size: cover;
}
</style>
