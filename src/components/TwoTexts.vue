<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  props: {
    head: String,
    text: String,
    className: String
  }
})
</script>
<template>
  <h2 :class="className">{{ head }}</h2>
  <p :class="className">{{ text }}</p>
</template>

<style scoped>
h2.small {
  font-size: 1.7rem;
}

p.small {
  font-size: 1.2rem;
}

h2,
p {
  text-align: center;
}

p {
  font-size: 1.6rem;
  padding: 0 14rem;
}
</style>