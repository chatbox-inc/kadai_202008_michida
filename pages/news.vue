<template>
  <div class="container-fluid">
    <div class="news-top-area">
      <div class="news-top-text-area">
        <h1>NEWS</h1>
        <p>-ニュース-</p>
      </div>
    </div>
    <hr />
    <div class="row">
      <div class="news-main-box col-md-9">
        <div class="article-tag">
          <span>リクルート</span>
          <span>2020.07.13</span>
        </div>
        <h2>オンライン会社説明会について</h2>
        <img src="/images/onlineSeminar.png" alt="オンライン会社説明会" />
        <p>各回、先着申し込み順(人数制限あり)</p>
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
          その他詳細はマイナビよりご予約後、受付メールに記載の【参加手引】にてご確認ください。
        </p>
        <div class="link-box">
          <a href="#">マイナビで日時確認・予約する</a>
        </div>
      </div>
      <aside class="category col-md-3">category</aside>
      <hr />
      <div class="link-box">
        <a href="#">ニュース一覧に戻る</a>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "~assets/scss/common.scss";
.container-fluid {
  .news-top-area {
    background-image: url("/images/company.jpg");
    background-size: cover;
    @include sp {
      height: 200px;
    }
    .news-top-text-area {
      text-align: center;
    }
  }
  .news-main-box {
  }
  .category {
    @include sp {
      display: none;
    }
  }
}
</style>
