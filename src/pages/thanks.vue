<template>
  <section id="thanks">
    <div class="thanks">
      <h2>Complete!</h2>
      <div class="text">
        <p>
          The Thinkerをプレイして頂きありがとうございました．
          <br />アンケートにご協力いただけると幸いです．
        </p>
      </div>
      <div class="selection">
        <v-btn color="#E8B96D" dark large to="https://forms.gle/o76ngA77m89A3awj9">アンケートへ</v-btn>
        <v-btn color="#E8B96D" dark large to="/">トップへ</v-btn>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "ThanksPage"
});
</script>

<style lang="scss" scoped>
.thanks {
  text-align: center;
  margin: 0 auto;
  margin-top: 40%;
  width: 80%;
  h2 {
    font-family: "PixelMplus12";
    font-size: 3rem;
    color: #e8b96d;
  }
  .text {
    margin-top: 2%;
    p {
      font-family: "PixelMplus10";
      font-size: 20px;
      color: #fff;
    }
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
    }
  }
}
</style>
