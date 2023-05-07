<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    header: {
      type: Object,
      required: true
    },
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
      <component :is="header" />
      <p>{{ text }}</p>
      <button class="btn">{{ btnText }}</button>
    </div>
    <div class="media">
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

/* @media screen and (max-width: 1024px) {
  section {
    flex-direction: column;
  }

  section div {
    width: 100%;
  }

  .texts {
    order: 2;
  }
} */
</style>