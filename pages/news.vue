<template>
  <div class="news-container">
    <div class="news-top-area">
      <div class="news-top-text-area">
        <h1>NEWS</h1>
        <p>-ニュース-</p>
      </div>
    </div>
    <div class="news-row">
      <div class="news-main-box">
        <div class="article-tag">
          <span class="tag">リクルート</span>
          <span>2020.07.13</span>
        </div>
        <h2>オンライン会社説明会について</h2>
        <img src="/images/onlineSeminar.png" alt="オンライン会社説明会" />
        <p class="seminar-end">各回、先着申し込み順(人数制限あり)</p>
        <p>
          採用担当が会社概要・募集要項・選考方法・ゲーム制作のスタンス等、
          よりグッド・フィールへの理解を深めていただく場としてオンライン会社説明会を開催します。
        </p>
        <h3>募集職種</h3>
        <p>デザイナー、プランナー、プログラマー</p>
        <h3>配信方法</h3>
        <p>Zoomアプリを使用したリアルタイム配信</p>
        <h3>視聴方法</h3>
        <p>説明会当日に【マイナビお返事箱】へZoom【ミーティングID】送付いたします。</p>
        <ul class="notice">
          <li>※開始10分前にはアクセスしてください。</li>
        </ul>
        <h3>開催日時・予約</h3>
        <p>
          マイナビにて開催日時をご確認いただきご予約ください。
          <br />その他詳細はマイナビよりご予約後、受付メールに記載の【参加手引】にてご確認ください。
        </p>
        <div class="link-box-book">
          <a href="#">マイナビで日時確認・予約する</a>
        </div>
      </div>
      <aside class="category">
        <h4>CATEGORY</h4>
        <a href="#">
          <span>すべて</span>
        </a>
        <br />
        <a href="#">
          <span>コーポレート</span>
        </a>
        <br />
        <a href="#">
          <span>リクルート</span>
        </a>
        <br />
        <a href="#">
          <span>ゲーム</span>
        </a>
        <hr />
        <a href="#">
          <span>すべて</span>
        </a>
        <a href="#">
          <span>2020</span>
        </a>
        <br />
        <a href="#">
          <span>2019</span>
        </a>
      </aside>
    </div>
    <div class="link-box-back">
      <a href="#">ニュース一覧に戻る</a>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "~assets/scss/common.scss";
.news-container {
  background-color: rgba(221, 221, 221, 0.6);
  font-size: 12px;
  font-weight: bolder;
  @include pc {
    font-size: 13px;
  }
}
.news-top-area {
  display: flex;
  justify-content: space-between;
  margin-top: 60px;
  height: 200px;
  background-image: url("/images/company.jpg");
  background-size: cover;
  padding-top: 40px;
  @include pc {
    margin: 0;
    height: 430px;
  }
}
.news-top-text-area {
  padding-top: 30px;
  text-align: center;
  width: 50%;
  height: 70%;
  margin: 0 auto;
  background-color: #fff;
  border-radius: 30px;
  opacity: 0.8;
  @include pc {
    margin: 120px auto;
    width: 25%;
    height: 35%;
  }
}
.news-top-text-area h1 {
  font-size: $font-A;
  margin: 0;
  @include bold;
  @include pc {
    font-size: $font-B;
  }
}
.news-top-text-area p {
  margin: 0;
  @include bold;
}
//記事部分
.news-row {
  @include pc {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
  }
}
.news-main-box {
  background: #fff;
  width: 95%;
  padding: 30px 10px;
  margin: 20px auto;
  border-radius: 10px;
  @include pc {
    flex: 3;
    padding: 40px;
  }
}
.article-tag .tag {
  color: #fff;
  margin-top: 8px;
  margin-bottom: 8px;
  font-size: 12px;
  padding: 4px 30px;
  background: #ffb32e;
  border-radius: 30px;
}
h2 {
  @include bold;
  font-size: 16px;
  border-bottom: 1px solid #ddd;
  padding-bottom: 10px;
  margin-top: 15px;
  margin-bottom: 15px;
  @include pc {
    font-size: $font-B;
  }
}
.seminar-end {
  color: #fff;
  padding: 5px 8px;
  margin: 15px 0;
  background: crimson;
  border-radius: 4px;
}
h3 {
  @include bold;
  font-size: 16px;
  margin: 30px 0 30px 0;
  border-left: solid 5px #ffb32e;
  padding-left: 10px;
  @include pc {
    font-size: $font-A;
  }
}
.notice {
  color: crimson;
}

.link-box-book {
  text-align: center;
  margin-top: 40px;
  margin-bottom: 40px;
  @include pc {
    margin-top: 60px;
  }
}
.link-box-book a {
  @include link-box(20px, 100px, 30px);
  @include pc {
    font-size: $font-A;
    @include link-box(40px, 100px, 80px);
  }
}
.link-box-back {
  text-align: center;
  margin-top: 60px;
  padding-bottom: 60px;
}
.link-box-back a {
  @include link-box(20px, 60px, 30px);
}
.category {
  display: none;
  @include pc {
    background: #fff;
    height: 330px;
    display: block;
    flex: 0.6;
    width: 100px;
    padding: 20px;
    margin: 20px 30px;
    border-radius: 10px;
  }
}
.category h4 {
  font-size: $font-A;
  @include bold;
}
.category span {
  display: inline-block;
  padding: 2px 20px;
  margin-bottom: 10px;
  background: rgba(221, 221, 221, 0.4);
  border-radius: 30px;
}
</style>
