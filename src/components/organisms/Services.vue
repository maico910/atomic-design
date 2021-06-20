<template>
  <div class="services">
    <Service
      title="Front End"
      description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis."
    />

    <Service
      title="Back End"
      description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis."
    />

    <Service
      title="Manutenção"
      description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis."
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
