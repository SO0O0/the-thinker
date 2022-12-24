<template>
  <section id="top-page">
    <div class="title">
      <h1>The Thinker</h1>
      <p>
        このアプリケーションは，
        <br />リサイクルに対する正しい疑問を持たせることを
        <br />目的としたシミュレーションゲームです．
      </p>
    </div>
    <div class="start">
      <v-btn color="#E8B96D" dark large to="/stage1">start</v-btn>
    </div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage"
});
</script>

<style lang="scss" scoped>
#top-page {
  height: 100vh;
  background-color: #184442;
  text-align: center;

  .title {
    margin-top: 70%;
    h1 {
      font-family: "PixelMplus12";
      font-size: 3rem;
      color: #fff;
    }

    p {
      font-family: "PixelMplus10";
      font-size: 15px;
      color: #e7e4e6;
      margin-top: 40px;
    }
  }

  .start {
    margin-top: 40px;

    .v-btn {
      font-family: "PixelMplus10";
      font-size: 15px;
      color: #000;
      background-color: #e8b96d;
      border-radius: 0;
      width: 120px;
      height: 50px;
    }
  }
}
</style>
