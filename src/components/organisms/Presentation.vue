<template>
  <div class="presentation">
    <social-network />
    <img
      class="presentation"
      src="@/assets/images/presentation.svg"
      alt="Apresentação"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialNetwork } from '@/components/molecules'

export default defineComponent({
  components: {
    SocialNetwork
  }
})
</script>

<style lang="scss" scoped>
.presentation {
  position: relative;
  display: grid;
  justify-content: center;
  .presentation {
    width: 80%;
    justify-self: center;
  }
  .social-networks {
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
  }
}
</style>
