<script setup lang="ts">
import Twotexts from './TwoTexts.vue'
</script>


<template>
  <section>
    <div>
      <Twotexts head="Sign up to our newsletter" text="Get early access to our news & releases" className="small" />
    </div>
    <form>
      <input type="text" placeholder="Enter your Email Address">
      <button class="btn">Sign Up</button>
    </form>
  </section>
</template>

<style scoped>
section {
  padding: 4rem 0;
  border-top: 1px dashed var(--color-purple-light);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

form {
  margin-top: 3rem;
  width: 100%;
  max-width: 700px;
  background-color: #120F24;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  padding-left: 0;
}

input {
  padding: 1.2rem;
  width: -webkit-fill-available;
}

input::placeholder,
input {
  color: var(--color-text);
  font-size: 1rem;
}

button {
  background-color: var(--color-purple-light);
  color: var(--color-text);
  white-space: nowrap;
  /* height: max-content; */
}
</style>