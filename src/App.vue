<script setup lang="ts">

import Banner from './components/Banner.vue';
import Contact from './components/Contact.vue';
import DataImg from './components/DataImg.vue';
import Footer from './components/Footer.vue';
import RewardTokens from './components/RewardTokens.vue';
import Social from './components/Social.vue';

import Cards from './components/media/Cards.vue'
import Cube from './components/media/Cube.vue'
import Map from './components/media/Map.vue'

import Data1 from './components/headings/Data1.vue'
import Data2 from './components/headings/Data2.vue'
import Data3 from './components/headings/Data3.vue'
</script>

<template>
  <header>
    <nav>
      <div class="logo">
        <h1>R</h1>
        <h2>Reward.io</h2>
      </div>
      <ul>
        <li><button>Play</button></li>
        <li><button>Wallet</button></li>
        <li><button>Reward</button></li>
        <li><button>Roadmap</button></li>
        <li><button>Community</button></li>
      </ul>
      <div class="btns">
        <button>Login</button>
        <button class="btn ">Register</button>
      </div>
    </nav>
  </header>

  <div class="home">

    <DataImg :header="Data1"
      text="Connect to our DEX service and contribute to earn crypto & cash seamlessly. Anyone can earn crypto by learning how to use blockchain products and completing real-time tasks."
      btnText="Get Started" imgSrc="../assets/vid.gif" sectionName="no-pb" :mediaComponent="Cube" />
    <div class="box">
      <span>Questions? Talk to an expert <img src="./assets/arrow-right.svg" alt="right arrow "></span>
      <div class="scroll">

        <img src="./assets/scroll.gif" alt="scroll down indicator">
      </div>
    </div>
  </div>

  <Banner />
  <DataImg :header="Data2"
    text="Our platform reaches people all over the world, we will help you in growing your knowledge about the crypto space and earn at the same time. Complete quests to earn experience points, skill points and guild coin tokens."
    btnText="Play Now" :mediaComponent="Map" />
  <DataImg :header="Data3"
    text="Our platform provides maximum security for our users through a safe transaction security, unique smart wallet card and embedded fintech experience to help you grow."
    btnText="Create Wallet" className="right" :mediaComponent="Cards" />
  <RewardTokens />
  <Social />
  <Contact />
  <Footer />
</template>

<style  scoped>
ul,
nav,
.logo,
.btns {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav {
  width: 100%;
  font-weight: bold;
  padding: 0 4rem;
  min-width: 1024px;
}

.logo {
  gap: 3px
}

h1 {
  font-size: 2rem;
}

h2 {
  font-weight: 300;
  font-size: 1.3rem;
}

ul {
  justify-content: space-evenly;
}

ul li {
  margin: 0 1rem;
  padding: 0 .2rem;
}

button {
  font-size: 1.2rem;
  font-weight: 500;
}

.btns {
  gap: 7px;
}

.btns button:first-child {
  padding: 0 1.5rem;
}

.home {
  height: 95vh;
  min-height: 800px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.box {
  padding: 1rem 4rem;
}

@media screen and (max-width: 1024px) {
  .box {
    padding: 1rem 2.4rem;
  }

  nav {
    padding-left: 2.4rem;
    padding-right: 2.4rem;
  }

  ul li {
    margin: 0 .4rem;
    padding: 0 .2rem;
  }

}

.box span {
  display: flex;
  align-items: center;
  gap: 4px;
}

.box span img {
  animation: glow 3s ease-in infinite backwards;
}

.scroll {
  display: flex;
  width: 100%;
  justify-content: center;
}

.scroll img {
  width: 150px;
}

@keyframes glow {
  0% {
    filter: brightness(100%);
  }

  50% {
    filter: brightness(0);
  }

  10% {
    filter: brightness(100%);
  }
}
</style>
