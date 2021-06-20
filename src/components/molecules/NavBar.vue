<template>
  <nav class="nav-bar">
    <NavItem
      v-for="(item, index) in items"
      :key="index"
      :text="item.text"
      :to="item.to"
    />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { NavItem } from '@/components/atoms'

export default defineComponent({
  components: {
    NavItem
  },
  data() {
    return {
      items: [
        { text: 'Serviços', to: '/services' },
        { text: 'Sobre mim', to: '/about' },
        { text: 'Cases', to: '/cases' },
        { text: 'Contato', to: '/contact' }
      ]
    }
  }
})
</script>

<style lang="scss" scoped>
.nav-bar {
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2rem;
}
</style>
