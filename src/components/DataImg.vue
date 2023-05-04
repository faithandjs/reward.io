<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    header: String,
    text: String,
    btnText: String,
    extraBten: Boolean,
    imgSrc: String,
    imgAlt: String,
    className: String,
    sectionName: String
  },

})

</script>

<template>
  <section :class="sectionName">
    <div :class="className">
      <h2>{{ header }}</h2>
      <p>{{ text }}</p>
      <button class="btn">{{ btnText }}</button>
    </div>
    <div>
      <!-- <img :src="require(imgSrc)" :alt="imgAlt" /> -->
    </div>
  </section>
</template>



<style scoped>
section {
  display: flex;
  align-items: center;
}

section.no-pb {
  padding-bottom: 0;
}

section div {
  width: 50%;
  display: grid;
  gap: 2.3rem;
  justify-content: center;
}

.right {
  order: 2;
}

/* h2 {
  font-size: 2.3rem;
  line-height: 1.5;
  padding-bottom: 1rem;
} */

/* p {
  font-weight: 300;
} */</style>