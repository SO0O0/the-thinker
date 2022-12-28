<template>
  <section class="result1">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        ディーゼル車を買った！
        <br />けど最近はガソリンが
        <br />高いな…
        <br />電気自動車の方が
        <br />良かったかも…
      </p>
    </div>
    <img src="~/assets/img/car.png" alt="car" />
    <div class="message">
      <p>
        エンジンでガソリンが燃料として，使用されると，CO2などの温室効果ガスが排出され，環境への負荷が大きくなります．
        <br />そのため，近年は電気自動車などの普及が進んでいますが，電気自動車もまた，製造の際の温室効果ガスの排出量が大きいことが指摘されています．
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
.result1 {
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
    width: 70%;
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
