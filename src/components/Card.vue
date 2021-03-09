<template>
  <div class="ctn">
    <div class="profile-pic">
      <div class="bg">
        <img src="../assets/image-victor.jpg" alt="" class="img" />
      </div>
      <div class="white-space"></div>
    </div>
    <div class="profile-info">
      <div class="name-age">
        <div class="name">Victor Crest</div>
        <div class="age">26</div>
      </div>
      <div>London</div>
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
};
</script>

<style lang="sass" scoped>

$dark-gray: hsl(0, 0%, 59%)

.ctn
  width: 22em
  border-radius: 1em

.name,
.age
  margin: 0.3em

.name
  font-weight: bold
  font-size: 18px

.bg
  background-image: url("../assets/bg-pattern-card.svg")
  background-size: contain
  height: 8.8rem
  border-radius: 1em 1em 0 0
  display: flex
  justify-content: center
  align-items: flex-end

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

.profile-info
  align-self: stretch
  display: flex
  flex-direction: column
  align-items: center
  padding: 1em

.profile-stats
  border-top: 1px solid gray
  display: flex
  justify-content: center
  padding: 1em


.stats-label-ctn
  padding: 1em
  display: flex
  flex-direction: column
  align-items: center


.label
  font-size: 0.8em
  letter-spacing: 2px
  color: $dark-gray


.stat
  font-weight: 700
  font-size: 18px
  padding: 0.5em
</style>
