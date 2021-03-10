<template>
  <div class="ctn">
    <div class="innerctn ctn-1"><img :src="topSVG" class="top-svg" /></div>
    <div class="innerctn ctn-2"></div>
    <div class="innerctn ctn-3"></div>
    <div class="innerctn ctn-4">
      <img :src="bottomSVG" class="bottom-svg" />
    </div>
  </div>
</template>

<script>
import Top from "../assets/bg-pattern-top.svg";
import Bottom from "../assets/bg-pattern-bottom.svg";
export default {
  name: "Background",
  computed: {
    topSVG() {
      return Top;
    },
    bottomSVG() {
      return Bottom;
    },
  },
};
</script>

<style lang="sass" scoped>

.ctn
    display: grid
    grid-template-columns: 50% 50%
    grid-template-rows: 50% 50%

.innerctn

.ctn-1
    align-self: end
    justify-self: end


.top-svg
    width: 70vw
    height: 70vw

.bottom-svg
    width: 70vw
    height: 70vw

@media screen and (max-width: 800px)
    .top-svg
        width: 100vw
        height: 100vw
        margin-bottom: 5em

    .bottom-svg
        margin-top: 5em
        width: 100vw
        height: 100vw
</style>
