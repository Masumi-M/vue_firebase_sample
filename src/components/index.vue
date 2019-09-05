<template>
  <div id="index">
    <h1>{{title}} Page</h1>
    <p>{{msg}}</p>
    <p>
      Link:
      <a v-bind:href="link" target="_blank">{{link}}</a>
    </p>
  </div>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      title: "Index",
      msg: "This is a sample page using vue.js and firebase.",
      link: "https://github.com/Masumi-M/vue_firebase_sample"
    };
  }
};
</script>

<style scoped lang="scss">
</style>
