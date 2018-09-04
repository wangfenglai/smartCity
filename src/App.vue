<template>
  <div id="app">
    <app-header></app-header>
    <router-view/>
    <app-aside></app-aside>
    <app-footer></app-footer>
  </div>
</template>

<script>
import AppHeader from '@/components/common/appheader'
import AppFooter from '@/components/common/appfooter'
import AppAside from '@/components/common/appaside'
export default {
  name: 'App',
  components: {AppHeader, AppFooter,AppAside}

}
</script>

<style>
@import "../base.css";

</style>
