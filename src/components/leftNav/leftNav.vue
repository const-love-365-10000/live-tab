<template>
  <div class="leftNav">
    <div class="userBox">
      <div>
        <img
          class="userHeaderImg"
          src="https://th.bing.com/th/id/OIP.SO720ddJeB077gpTU60t6wHaJe?pid=ImgDet&rs=1"
        />
      </div>
    </div>
    <nav class="tagNav">
      <ul class="tagUl">
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </nav>
  </div>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class leftNav extends Vue {}
</script>

<style lang="scss" scoped>
.leftNav {
  width: 70px;
  height: 100vh;
  background: #1e1e2e;

  .userHeaderImg {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    border: 2px outset;
    object-fit: cover;
  }
}
</style>