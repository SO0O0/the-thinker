<template>
  <section class="stage1-story">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        レジ袋一枚で
        <br />5円もした…
        <br />エコバッグを買った
        <br />ほうがいいのかな？
      </p>
    </div>
    <img src="~/assets/img/shopping-bag.png" alt="hungry" />
    <div class="message">
      <p>
        レジ袋などのプラスチックが
        <br/>環境に与える負荷から，
        <br />近年はレジ袋の有料化が進んでいます．
        <br />しかし，エコバッグもまた製造時に
        <br />多大な環境負荷がかかっていることが
        <br />指摘されています．
        <br />どちらを選ぶべきか，考えてみましょう．
      </p>
    </div>
    <div class="link">
      <nuxt-link to="stage1-story">戻る</nuxt-link>
      <nuxt-link to="/">TOP</nuxt-link>
      <nuxt-link to="stage2-story">次へ</nuxt-link>
    </div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Stage1Story"
});
</script>

<style lang="scss" scoped>
.stage1-story {
  text-align: center;
  .proposal {
    position: relative;
    margin-top: 10%;
    img {
      width: 75%;
    }
    p {
      position: absolute;
      top: 43%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-family: "PixelMplus10";
      font-size: 20px;
    }
  }
  img {
    width: 80%;
  }
  .selection {
    margin-top: 2%;
    display: inline-flex;
    flex-direction: column;
    .v-btn {
      margin-bottom: 20px;
      font-family: "PixelMplus10";
      font-size: 15px;
      color: #000;
      background-color: #e8b96d;
      border-radius: 0;
      width: 220px;
      height: 50px;
    }
  }

  .message {
    margin: 0 auto;
    margin-top: 10%;
    width: 80%;
    background-color: #e8b96d;
    border-radius: 10px;
    box-shadow: 0 0 10px #000;
    p {
      font-family: "PixelMplus10";
      font-size: 15px;
      padding: 10px;
    }
  }

  .link {
    margin-top: 30px;
    display: grid;
    grid-template-columns: 10fr 1fr 10fr;

    a {
      font-family: "PixelMplus10";
      font-size: 15px;
      color: #FFF;
      text-decoration: none;
    }
  }
}
</style>
