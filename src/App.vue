<template>
  <div id="app">
    <menu-component></menu-component>
  </div>
</template>

<script>
import Menu from './components/Menu/Menu.vue'
export default {
  name: 'app',
  components: {
    MenuComponent: Menu,
  }
}
</script>
