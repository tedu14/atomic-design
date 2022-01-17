<template>
  <a class="nav-item" :href="link">
    {{ label }}
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    text: {
      type: String,
      required: true
    },
    to: {
      type: String,
      required: true
    }
  },
  computed: {
    link() {
      return this.to
    },
    label() {
      return this.text
    }
  }
})
</script>

<style lang="scss" scoped>
.nav-item {
  color: #293947;
  text-decoration: none;
  font-size: 1.3rem;
}
</style>
