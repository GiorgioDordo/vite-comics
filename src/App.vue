<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppNavbar from './components/AppNavbar.vue'
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
    AppNavbar,
    AppInfo,
    AppFooter
  }
}
</script>

<template>
<AppHeader />
<AppContent />
<AppNavbar />
<AppInfo />
<AppFooter />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./styles/general.scss" as *;
</style>
