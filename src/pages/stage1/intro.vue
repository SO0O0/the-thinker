<template>
  <section id="top-page">
    <div class="title">
      <h1>1st STAGE</h1>
      <h2>episode 買い物</h2>
    </div>
    <div class="start">
      <v-btn color="#E8B96D" dark large to="/stage1/intro">次へ</v-btn>
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
    margin-top: 260px;

    h1 {
      font-family: "PixelMplus12";
      font-size: 3rem;
      color: #fff;
    }

    h2 {
      font-family: "PixelMplus12";
      font-size: 1.5rem;
      color: #fff;
      margin-top: 40px;
    }
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
</style>
