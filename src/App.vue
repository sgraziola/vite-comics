<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import SiteFooter from './components/SiteFooter.vue';
import CallToAction from './components/CallToAction.vue';

export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter,
    CallToAction
  }

}
</script>

<template>
  <SiteHeader></SiteHeader>
  <!-- /#site_header -->
  <SiteMain></SiteMain>
  <CallToAction></CallToAction>

  <!-- /#site_main -->
  <SiteFooter></SiteFooter>
  <!-- /#site_footer -->

</template>

<style>

</style>