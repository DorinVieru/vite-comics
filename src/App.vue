<!-- SEZIONE JS SCRIPT -->
<script>

// IMPORTO LE COMPONTENTI
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<!-- SEZIONE HTML -->
<template lang="">
  <div>
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

<!-- SEZIONE STYLE -->
<style lang="scss">
  @use './styles/partials/variables' as *;
  @use './styles/generals.scss' as *;


</style>
