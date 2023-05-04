<script   lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    num: Number,
    head: String,
    text: String,
    btnText: String
  },

})

</script>

<template>
  <div class="card">
    <span>{{ num }}</span>
    <div>
      <h3>{{ head }}</h3>
      <p>{{ text }}</p>
      <button>{{ btnText }}</button>
    </div>

  </div>
</template>

<style scoped>
.card,
.card div {

  display: flex;
  flex-direction: column;
}

.card {
  width: 400px;
  height: 270px;
  flex-shrink: 0;
  position: relative;
  overflow: hidden;
  border: 1px solid var(--color-purple-light);
}

.card::after {
  content: ' ';
  position: absolute;
  width: 70px;
  height: 70px;
  bottom: 0;
  right: -35px;
  transform: rotate(45deg) translate(50%, 50%);
  background-color: var(--color-purple-light);
}

.card div {
  height: 90%;
  justify-content: space-between;
  align-items: center;
  padding: 1.5rem 1rem;
}

span {
  width: 30px;
  height: 30px;
  flex-shrink: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: bold;
  background-color: var(--color-purple-light);
}

h3 {
  font-size: 1.6rem;
}

p {
  font-weight: 300;
  text-align: center;
}

button {
  font-weight: bold;
  color: var(--color-purple-light);
}
</style>
