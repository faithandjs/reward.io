<template>
  <section>
    <div class="banner-style"></div>
    <div class="banner-bg">
      <img src="../assets/forbes.svg" alt="forbes logo"><img src="../assets/polygon.svg" alt="polygon logo"><img
        src="../assets/coinbase.svg" alt="coinbase logo"><img src="../assets/binance.svg" alt="binance logo"><img
        src="../assets/business.svg" alt="business insider logo">
    </div>
  </section>
</template>


<style  scoped>
section {
  position: relative;
  margin: 2rem 0;
  padding: 0;
}

.banner-style {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 120vw;
  height: 105%;
  z-index: -1;
  transform: rotate(3deg) translate(-50%, -15%);
  background-color: var(--color-purple-light);
}

.banner-bg {
  display: flex;
  justify-content: space-between;
  padding: 3rem 4rem;
  background-color: var(--color-text);
}
</style>