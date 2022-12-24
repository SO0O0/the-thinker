<template>
  <section class="stage1-story">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        お腹減ったなあ
        <br />お弁当買いに行こう
        <br />でもエコバッグ
        <br />持ってない…
      </p>
    </div>
    <img src="~/assets/img/hungry.png" alt="hungry" />
    <div class="selection">
      <v-btn color="#E8B96D" dark large to="/stage1-result">レジ袋を買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage1-result">エコバックを買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage1-result">手で持って帰る</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage1-result">ご飯を食べるのを止める</v-btn>
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
  height: 100vh;
  .proposal {
    position: relative;
    margin-top: 10%;
    img {
      width: 75%;
    }
    p {
      top: 40px;
      left: 105px;
      position: absolute;
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
}
</style>
