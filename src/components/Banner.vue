<template>
  <section>
    <div class="banner-bg">
      <div class="banner-style"></div>
      <div class="band">
        <img src="../assets/forbes.svg" alt="forbes logo">
        <img src="../assets/polygon.svg" alt="polygon logo">
        <img src="../assets/coinbase.svg" alt="coinbase logo">
        <img src="../assets/binance.svg" alt="binance logo">
        <img src="../assets/business.svg" alt="business insider logo">
      </div>
    </div>
  </section>
</template>


<style  scoped>
section {
  margin: 2rem 0;
  position: relative;
  padding: 0;
  overflow-x: clip;
}

.banner-style {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 105vw;
  height: 105%;
  z-index: -1;
  transform: rotate(3deg) translate(-50%, -20%);
  background-color: var(--color-purple-light);
}

.band {
  padding: 3rem 4rem;
  background-color: var(--color-text);
  overflow: scroll;
  justify-content: space-between;
  display: flex;
  gap: 30px;
  flex-wrap: nowrap;
}

@media screen and (max-width: 1024px) {
  .band {
    padding: 2rem 1.4rem;
  }

  .banner-style {
    display: none;
  }
}
</style>