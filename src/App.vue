<script>
import AppHeader from './components/AppHeader.vue'
import AppJambo from './components/AppJambo.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppJambo,
    AppFooter,
  }
}
</script>
<template>
  <AppHeader />
  <AppMain />
  <AppJambo />
  <AppFooter />
</template>
<style scoped></style>
