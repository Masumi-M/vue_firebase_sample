<template>
  <div id="index">
    <div class="ui vertical green sidebar menu">
      <a class="header item sidebarLogo" href="/index.php">
        <div class="ui image">
          <img src="/Resource/img/small_only_image.svg">
        </div>umi-mori
      </a>
      <a class="item" href="/home.php">
        <i class="home icon"></i>Home
      </a>
      <a class="item" href="/product.php">
        <i class="code icon"></i>Product
      </a>
      <a class="item" href="/article.php">
        <i class="newspaper icon"></i>Article
      </a>
      <a class="item" href="/blog.php">
        <i class="paint brush icon"></i>Blog
      </a>
    </div>

    <div class="pusher" id="MainBody">
      <div class="ui container">
        <div id="NavMenu">
          <div class="ui large secondary menu">
            <a class="toc item">
              <i class="sidebar icon"></i>
            </a>
            <a class="header item mainbarLogo" href="/index.php">
              <div class="ui image">
                <img src="/Resource/img/small_only_image.svg">
              </div>umi-mori
            </a>
            <a class="item PCMenu" href="/home.php">
              <i class="home icon"></i>Home
            </a>
            <a class="item PCMenu" href="/product.php">
              <i class="code icon"></i>Product
            </a>
            <a class="item PCMenu" href="/article.php">
              <i class="newspaper icon"></i>Article
            </a>
            <a class="item PCMenu" href="/blog.php">
              <i class="paint brush icon"></i>Blog
            </a>
          </div>
        </div>
        <div id="RightMenu">
          <div class="ui dropdown item">
            <i class="share alternate icon"></i>
            <div class="menu">
              <a
                class="item"
                href="https://itunes.apple.com/jp/developer/masumi-morishige/id1437701072"
                target="_blank"
              >
                <i class="app store ios icon"></i>apple-store
              </a>
              <a
                class="item"
                href="https://play.google.com/store/apps/dev?id=6043692952300374835"
                target="_blank"
              >
                <i class="google play icon"></i>google-play
              </a>
              <a class="item" href="https://twitter.com/umi_mori_jp" target="_blank">
                <i class="twitter icon"></i>twitter
              </a>
              <a
                class="item"
                href="mailto:masumi.developer@gmail.com?subject=ポートフォリオからのお問い合わせ&body=【氏名】：%0D%0A【概要】：%0D%0A【本文】：%0D%0A"
              >
                <i class="envelope icon"></i>mail
              </a>
              <a class="item" href="https://qiita.com/umi_mori" target="_blank">
                <i class="search icon"></i>qiita
              </a>
              <a class="item" href="https://github.com/Masumi-M" target="_blank">
                <i class="github icon"></i>github
              </a>
            </div>
          </div>

          <div id="smallFlag">
            <div class="ui button green" onclick="jumpToSupport()">
              <i class="flag icon"></i>
            </div>
          </div>

          <div class="ui labeled button small" id="bigFlag" tabindex="0" onclick="jumpToSupport()">
            <div class="ui green button small">
              <i class="flag icon"></i>
            </div>
            <a class="ui basic green left pointing label small">Support</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<style scoped lang="scss">
</style>
