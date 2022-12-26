<template>
  <section class="result2">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        エコバッグを買ったけど
        <br />結構しっかりしてるな…
        <br />作るの大変そうだぞ…
      </p>
    </div>
    <img src="~/assets/img/eco-bag.png" alt="hungry" />
    <div class="message">
      <p>
        レジ袋の代わりにエコバッグを使うことで
        <br />環境への負荷が減ると思っていませんか？
        <br />エコバッグの生産・輸送は,レジ袋よりもCO2などのエネルギーの排出量が大きいことが指摘されています．
        <br />エコバッグを本当に使うべきなのか，慎重に考えてみましょう．
      </p>
    </div>
    <div class="link">
      <nuxt-link to="/stage1/story">戻る</nuxt-link>
      <nuxt-link to="/">TOP</nuxt-link>
      <nuxt-link to="/stage2/intro">次へ</nuxt-link>
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
.result2 {
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
      font-size: 17px;
    }
  }
  img {
    width: 80%;
  }

  .message {
    margin: 0 auto;
    margin-top: 15px;
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
    margin-bottom: 45px;
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
