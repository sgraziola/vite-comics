<script>
import CallToAction from './CallToAction.vue';
export default {
    name: "SiteMain",
    components: {
        CallToAction,
    }
}

</script>
<template>

    <main id="site_main">
        <div class="container d-flex">
            --> Content Goes Here &lt--
        </div>
        <CallToAction />
    </main>

</template>

<style lang="scss" scoped>
.container {
    height: 150px;
}
</style>