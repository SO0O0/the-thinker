<template>
  <section class="story">
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
      <v-btn color="#E8B96D" dark large to="/stage1/result1">レジ袋を買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage1/result2">エコバックを買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage1/result3">手で持って帰る</v-btn>
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
.story {
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
    margin-top: 30px;
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
