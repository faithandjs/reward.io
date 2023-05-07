<template>
  <div>
    <img src="../../assets/bottom-card.png" alt="grey reward.io card" class="bottom">
    <img src="../../assets/top-card.png" alt="white reward.io card" class="top">
  </div>
</template>

<style scoped>
div {
  position: relative;
  width: 50%;
}

img {
  position: absolute;
}

.top {
  left: 100px;
  top: -125px;
}

.bottom {
  left: 0;
  top: -160px;
}

@media screen and (max-width: 1024px) {
  div {
    left: -30px;
  }

  .top {
    left: 50px;
    top: -125px;
  }
}
</style>