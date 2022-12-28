<template>
  <section class="story">
    <div class="proposal">
      <img src="~/assets/img/hukidashi.png" alt="hukidashi" />
      <p>
        ついに憧れの
        <br />マイカーを買うぞ！
        <br />どんな車にしようかな？
      </p>
    </div>
    <img src="~/assets/img/think.png" alt="think" />
    <div class="selection">
      <v-btn color="#E8B96D" dark large to="/stage2/result1">ディーゼル車を買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage2/result2">電気自動車を買う</v-btn>
      <v-btn color="#E8B96D" dark large to="/stage2/result3">水素自動車を買う</v-btn>
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
      font-size: 17px;
    }
  }
  img {
    width: 50%;
    margin: 0 auto;
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
