

<template>
  <section class="with-cards">

    <h2 class="head">How the Reward Token works</h2>
    <div class="cards">
      <Card :num='1' head="Complete task"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="View All Tasks" />
      <Card :num="2" head="Connect Wallet"
        text="After the completion of a task, users are able to connect their wallet which help save users tokens & earnings."
        btnText="Connect Wallet" />
      <Card :num="3" head="Gain Crypto XP"
        text="Afters users have been able to earn while performing tasks, they gain crypto experience alongsides."
        btnText="Check XP Level" />
      <Card :num="4" head="Withdrawal"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="How to Withdraw" />
    </div>
  </section>
  <Tokens />
  <section class="with-cards">
    <div class="head">

      <Twotexts head="Roadmaps"
        text="The complete path to improving the utility and features of the platform for our users." />
    </div>
    <div class="cards">
      <Card :num="1" head="Q1 2022"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="View All Tasks" />
      <Card :num="2" head="Q2 2022"
        text="After the completion of a task, users are able to connect their wallet which help save users tokens & earnings."
        btnText="Connect Wallet" />
      <Card :num="3" head="Q3 2022"
        text="Afters users have been able to earn while performing tasks, they gain crypto experience alongsides."
        btnText="Check XP Level" />
      <Card :num="4" head="Q4 2022"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="How to Withdraw" />
      <Card :num="5" head="Q1 2023"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="How to Withdraw" />
      <Card :num="6" head="Q2 2023"
        text="Users complete tasks in order to earn token points, gain crypto experience & also earn tokens."
        btnText="How to Withdraw" />
    </div>

  </section>
</template>

<script setup lang="ts">
import Card from './Card.vue'
import Twotexts from './TwoTexts.vue'
import Tokens from './Tokens.vue'
</script>
<style scoped>
section.with-cards {
  padding: 0;
}

.cards {
  overflow: scroll;
  padding: 0 2.4rem;
  display: flex;
  gap: 20px;
  flex-wrap: nowrap;
}

.head {
  padding-bottom: 2.3rem;
}

h2 {
  text-align: center;
  padding-bottom: 10px;
}
</style>