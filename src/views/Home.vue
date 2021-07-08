<template>
  <div class="home" :style="{ background: 'url(' + backgroundImgUrl + ')' }">
    <!-- 主要显示的左边标签栏和右边主页 -->
    <main class="main">
      <left-nav></left-nav>
    </main>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

import leftNav from "@/components/leftNav/leftNav.vue";

@Options({
  components: { leftNav },
  computed: {
    backgroundImgUrl() {
      console.log();

      return (
        // "https://source.unsplash.com/random/" +
        "https://picsum.photos/" +
        window.innerWidth +
        // "x"
        "/" +
        window.innerHeight
      );
    },
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
.home {
  width: 100vw;
  height: 100vh;
}
.main {
  display: flex;
}
</style>
