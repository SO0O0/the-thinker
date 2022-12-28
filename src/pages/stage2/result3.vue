<template>
  <section class="result3">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        水素自動車を買ったけど，
        <br />充電できる場所がない…
        <br />失敗だったかな…
      </p>
    </div>
    <img src="~/assets/img/car.png" alt="hungry" />
    <div class="message">
      <p>
        水素自動車はディーゼル車に比べてCO2排出量が少なく，環境に優しいとされています．
        しかし，水素自動車の燃料となる水素は石油や天然ガスなどの化石燃料を基に作られるのが一般的であり，CO2が排出されないわけではありません．
        <br />ディーゼル車，電気自動車，水素自動車，どれが環境に優しいか，慎重に考えてみましょう．
      </p>
    </div>
    <div class="link">
      <nuxt-link to="/stage2/story">戻る</nuxt-link>
      <nuxt-link to="/">TOP</nuxt-link>
      <nuxt-link to="/thanks">次へ</nuxt-link>
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
.result3 {
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
