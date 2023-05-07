<template>
  <section>
    <div class="gif-header">
      <img src="../assets/arrowDown.gif" alt="">
      <h2>Reward.io Tokens</h2>
    </div>
    <div class="star">
      <img src="../assets/star.svg" alt="yellow star">
      <h3>Levels of the Reward Tokens.</h3>
    </div>

    <div class="main">
      <div class="text">
        <div class="head">
          <h2>Platinum Token</h2>
          <ul>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <p>Platinum tokens are given to users with wide range of the blockchain experience. They’re known to be masters of
          crypto.</p>
        <button>Coming Soon</button>
      </div>
      <div class="card">
        <img src="../assets/filled-card.png" alt="a giftcard">
      </div>
    </div>
    <div class="tokens">
      <img src="../assets/polygon-token.png" alt="polygon logo on a coin/token" class="first">
      <img src="../assets/binance-token.png" alt="binance logo on a coin/token" class="last">
    </div>
  </section>
</template>

<style scoped>
section {
  position: relative;
  margin-bottom: 50px;
}

.gif-header {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 6px;
}

.gif-header img {
  width: 2.3rem;
}

.star {
  margin: 2rem 0;
  width: max-content;
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1.2rem;
  padding-right: 10rem;
  border: 1px solid var(--color-purple-light);
}

h3 {
  font-size: 1.9rem;
}

.main {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.text {
  width: 55%;
  display: grid;
  gap: 3rem;
}

p {
  padding-right: 10rem;
}

.head ul {
  display: flex;
  width: 60%;
  gap: 10px;
}

.head ul li {
  width: 25%;
  height: 6px;
  background-color: #B9ABFF;
}

.head ul li:first-child {
  background-color: var(--color-purple-light);
}

button {
  padding: 0.8rem 2.5rem;
  background-color: #7B7785;
  color: #D2D2D2;
  font-size: 1.2rem;
}

.card {
  width: 40%;
  text-align: center;
}


.card img,
.tokens img {
  filter: grayscale(10);
  transition: all .2s;
}

.card img {
  transform: scale(.9);
}

.card img:hover,
.tokens img:hover {
  transform: scale(1);
  filter: grayscale(0);
}

.tokens img {
  position: absolute;
}

.first {
  top: 5rem;
  right: 5rem;
}
</style>