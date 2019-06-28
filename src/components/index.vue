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
