<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppHero from './components/AppHero.vue'
import AppInfo from './components/AppInfo.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  data() {
    return {
    }
  },
  components:{
    AppHeader,
    AppContent,
    AppHero,
    AppInfo,
    AppFooter
  }
}
</script>

<template>
<AppHeader />
<AppContent />
<AppHero />
<AppInfo />
<AppFooter />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./styles/general.scss" as *;
</style>
