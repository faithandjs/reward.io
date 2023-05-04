<template>
  <footer>
    <div class="logo">
      <h1>R</h1>
    </div>
    <div class="lists">
      <ul>
        <li class="head">Tokens</li>
        <li>Reward Coin</li>
        <li>Reward Gem</li>
        <li>Token Prize</li>
      </ul>
      <ul>
        <li class="head">Resources</li>
        <li>Whitepaper</li>
        <li>Blog</li>
        <li>FAQ</li>
      </ul>
      <ul>
        <li class="head">Developer</li>
        <li>Marketplace</li>
        <li>Protocol</li>
        <li>Contact</li>
      </ul>
    </div>
    <div class="rights">
      <p>© Reward 2022. All rights reserved.</p>
      <div>
        <img src="../assets/discord.svg" alt="discord logo"><img src="../assets/twitter.svg" alt="twitter logo"><img
          src="../assets/medium.svg" alt="medium logo"><img src="../assets/linkedin.svg" alt="linkein logo"><img
          src="../assets/youtube.svg" alt="youtube logo"><img src="../assets/facebook-logo.svg" alt="facebook logo"><img
          src="../assets/instagram.svg" alt="instagram logo">

      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4rem;
  padding-bottom: 7px;
}

h1 {
  font-size: 3rem;
}

.lists {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
}

.lists .head {
  font-size: 1.8rem;
  font-weight: bold;
}

li {
  font-size: 1.3rem;
  padding-bottom: 1rem;
}

.rights {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.rights p {
  font-size: 1.5rem;
}

.rights div img {
  width: 30px;
  margin: 0 1rem;
}

.rights div img:first-child,
.rights div img:nth-child(7) {
  width: 20px;
}
</style>