<script setup lang="ts">
import Twotext from './TwoTexts.vue'
</script>
<template>
  <section>
    <Twotext head="Community"
      text="Join a fast-growing community of players and earn a reward, connected all over the universe, building the new era of the Reward community." />
    <div>
      <img src="../assets/discord.svg" alt="discord logo"><img src="../assets/twitter.svg" alt="twitter logo"><img
        src="../assets/medium.svg" alt="medium logo"><img src="../assets/linkedin.svg" alt="linkein logo"><img
        src="../assets/youtube.svg" alt="youtube logo"><img src="../assets/facebook-logo.svg" alt="facebook logo"><img
        src="../assets/instagram.svg" alt="instagram logo">

    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 30px;

}

div {
  display: flex;
  align-items: center;
  gap: 30px;
  max-width: 70%;
}

div img {
  width: 40px;
}
</style>