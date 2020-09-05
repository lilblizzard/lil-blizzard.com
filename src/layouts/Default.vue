<template>
  <div class="layout">
    <Navbar />
    <slot />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
export default {
  components: {
    Navbar,
  },
}
</script>

<style>
body {
  font-family: 'Montserrat', sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
  background-color: black;
  color: white;
}
.layout {
  max-width: 50rem;
  margin: 0 auto;
  padding-left: 1rem;
  padding-right: 1rem;
}
</style>
