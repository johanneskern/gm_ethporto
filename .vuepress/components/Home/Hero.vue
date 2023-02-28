<template>
  <div class="hero-main">
    <div class="hero-main_headline">
        GM PORTO 2023
    </div>
    <div class="hero-main_headline-date">
      12. March - 19. March 2023
    </div>
    <div class="hero-main_headline-date">
        Bringing the first ETH event to the beautiful city of Porto.
    </div>
    <div class="hero-main_headline-date">
      This website allows anyone to add and update their side event.
    </div>
    <Button class="hero-main_button" buttonText="Submit Event" :to="this.config.themeConfig.nav[2].link" />
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

.hero-main
  color #fff
  display flex
  flex-direction column
  align-items center
  justify-content center
  padding 50px 0 0 0
  width 100%

  &_headline-date
    font-size clamp(1rem, calc(-0.875rem + 1.8vw), 8.5rem)
    line-height 28px
    margin-bottom 1rem
    padding 0 20px 0 20px
    text-align center

  &_headline
    font-size clamp(2.5rem, calc(-0.875rem + 8.333vw), 8.5rem)
    text-align center
    margin-bottom 1.5rem
    display flex
    justify-content center

  &_button
    padding-top 3rem

</style>
