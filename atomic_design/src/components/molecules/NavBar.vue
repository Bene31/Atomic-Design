<template>
  <nav class="nav-bar">
      <NavItem text="Serviços" to="/servicos" />
      <NavItem text="Sobre mim" to="/about" />
      <NavItem text="Cases" to="/cases" />
      <NavItem text="Contato" to="/contact" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import {NavItem} from '@/components/atoms'

export default defineComponent({
    /*props: {
        text: {type: String, required: true},
        to: {type: String, required: true}
    }*/
    components: {NavItem}
})
</script>

<style lang="scss" scoped>
  .nav-bar {
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>