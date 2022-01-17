<template>
  <a :href="link" class="social-link" target="_blank" rel="noopener noreferrer">
    <img :src="iconPath" :alt="alt" />
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    name: { type: String, required: true },
    icon: { type: String, required: true },
    to: { type: String, required: true }
  },
  computed: {
    iconPath() {
      return require(`@/assets/images/icons/${this.icon}`)
    },
    alt() {
      return this.name
    },
    link() {
      return this.to
    }
  }
})
</script>

<style lang="scss" scoped>
.social-link {
  background-color: #ff895f;
  width: 47px;
  height: 47px;
  border-radius: 5rem;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
  &:hover {
    transform: scale(1.1);
  }
  img {
    width: 23px;
    height: 23px;
  }
}
</style>
