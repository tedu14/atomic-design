<template>
  <div class="social-networks">
    <social-link
      icon="github.svg"
      name="Github"
      to="https://github.com/tedu14"
    />
    <social-link
      icon="twitter.svg"
      name="Twitter"
      to="https://github.com/tedu14"
    />
    <social-link
      icon="facebook.svg"
      name="Facebook"
      to="https://github.com/tedu14"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialLink } from '@/components/atoms'

export default defineComponent({
  components: {
    SocialLink
  }
})
</script>

<style lang="scss" scoped>
.social-networks {
  display: grid;
  grid-gap: 1rem;
}
</style>
