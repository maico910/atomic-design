<template>
  <div class="component">
    <Home />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Home } from '@/components/templates'

export default defineComponent({
  name: 'App',
  components: { Home }
})
</script>
