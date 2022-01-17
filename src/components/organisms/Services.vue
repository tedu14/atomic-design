<template>
  <div class="services">
    <service
      title="Front-end"
      description="Lorem ipsum dolor sit amet 
      consectetur adipisicing elit. Tenetur quo debitis deserunt id 
      laudantium eum, perspiciatis dolorem dolore consequuntur dolores laboriosam 
      fugit temporibus? Cum consequatur, facilis voluptatibus ullam odio eligendi?"
    />
    <service
      title="Back-end"
      description="Lorem ipsum dolor sit amet 
      consectetur adipisicing elit. Tenetur quo debitis deserunt id 
      laudantium eum, perspiciatis dolorem dolore consequuntur dolores laboriosam 
      fugit temporibus? Cum consequatur, facilis voluptatibus ullam odio eligendi?"
    />
    <service
      title="Mobile"
      description="Lorem ipsum dolor sit amet 
      consectetur adipisicing elit. Tenetur quo debitis deserunt id 
      laudantium eum, perspiciatis dolorem dolore consequuntur dolores laboriosam 
      fugit temporibus? Cum consequatur, facilis voluptatibus ullam odio eligendi?"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  components: {
    Service
  }
})
</script>

<style lang="scss" scoped>
.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}
</style>
