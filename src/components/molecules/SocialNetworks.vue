<template>
  <div class="social-networks">
    <SocialLink
      v-for="(link, index) in links"
      :key="index"
      :name="link.name"
      :to="link.to"
      :icon="link.icon"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialLink } from '@/components/atoms'

export default defineComponent({
  components: { SocialLink },
  data() {
    return {
      links: [
        { name: 'Github', to: 'https://github.com', icon: 'github.svg' },
        { name: 'Facebook', to: 'https://facebook.com', icon: 'facebook.svg' },
        { name: 'Twitter', to: 'https://twitter.com', icon: 'twitter.svg' }
      ]
    }
  }
})
</script>

<style lang="scss" scoped>
.social-networks {
  display: grid;
  grid-gap: 1rem;
}
</style>
