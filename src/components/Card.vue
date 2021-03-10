<template>
  <div class="ctn">
    <div class="profile-pic">
      <div class="bg">
        <!-- <Background class="background" /> -->
        <img src="../assets/image-victor.jpg" alt="" class="img" />
      </div>
      <div class="white-space"></div>
    </div>
    <div class="profile-info">
      <div class="name-age">
        <div class="name">Victor Crest</div>
        <div class="age">26</div>
      </div>
      <div class="location">London</div>
    </div>
    <div class="profile-stats">
      <div class="stats-label-ctn">
        <div class="stat">80K</div>
        <div class="label">Followers</div>
      </div>
      <div class="stats-label-ctn">
        <div class="stat">803K</div>
        <div class="label">Likes</div>
      </div>
      <div class="stats-label-ctn">
        <div class="stat">1.4K</div>
        <div class="label">Photos</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  components: {},
};
</script>

<style lang="sass" scoped>

$dark-gray: hsl(0, 0%, 59%)

.background
    position: absolute

.ctn
  width: 350px
  border-radius: 1em
  background: white

.name,
.age
  margin: 0.3em

.name
  font-weight: bold
  font-size: 18px

.age
    color: $dark-gray
    margin: 0 1em

.location
    color: $dark-gray
    font-size: .9em

.bg
  height: 8.8rem
  border-radius: 1em 1em 0 0
  display: flex
  justify-content: center
  align-items: flex-end
  background-image: url("../assets/bg-pattern-card.svg")

.img
  border-radius: 50%
  border: 5px solid white
  position: relative
  top: 58px
  width: 106px

.white-space
  height: 58px

.name-age
  display: flex
  align-items: center
  margin-bottom: .6em

.profile-info
  align-self: stretch
  display: flex
  flex-direction: column
  align-items: center
  padding: 1em 2em 1.5em

.profile-stats
  border-top: 1px solid $dark-gray
  display: flex
  justify-content: center
  padding: 1em


.stats-label-ctn
  padding: 1em
  display: flex
  flex-direction: column
  align-items: center


.label
  font-size: 0.65em
  letter-spacing: 1px
  color: $dark-gray


.stat
  font-weight: 700
  font-size: 18px
  padding: 0.4em 0.4em
</style>
