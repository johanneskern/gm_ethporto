<template>
  <div class="banner-main">
    <img class="banner-main_img" src="./../../public/eth-porto-banner.jpeg" alt="">
  </div>
</template>

<script>
import Button from "../Button.vue";
import themeConfig from "../../config";

export default {
  components: { Button },
  data() {
    return {
      config: themeConfig,
    };
  },
};
</script>

<style lang="stylus">
@import '../../theme/styles/config.styl'

.banner-main
  display flex
  align-items center
  justify-content center
  padding-top 150px

  &_img
    width 100%

</style>
