<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    header: String,
    text: String,
    btnText: String,
    extraBtn: Boolean,
    className: String,
    sectionName: String,
    mediaComponent: {
      type: Object,
      required: true
    }
  },

})

</script>

<template>
  <section :class="sectionName">
    <div :class='`${className} texts`'>
      <h2>{{ header }}</h2>
      <p>{{ text }}</p>
      <button class="btn">{{ btnText }}</button>
    </div>
    <div>
      <component :is="mediaComponent" />
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

}

.texts {
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