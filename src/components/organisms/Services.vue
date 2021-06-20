<template>
  <div class="services">
    <Service
      v-for="(service, index) in services"
      :key="index"
      :description="service.description"
      :title="service.title"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  components: {
    Service
  },
  data() {
    return {
      services: [
        {
          title: 'Front End',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis.'
        },
        {
          title: 'Back End',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis.'
        },
        {
          title: 'Manutençãp',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem eius nihil recusandae officiis, repudiandae quas error cumque assumenda deserunt. Minima velit maiores est. Ad illum culpa cumque ipsum numquam officiis.'
        }
      ]
    }
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
