<script>
import CallToAction from './CallToAction.vue'
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

        <CallToAction></CallToAction>
    </main>

</template>

<style lang="scss">
main {
    background-color: black;
    color: white;
    height: 150px;

    .container {
        height: 100%;
        align-items: center;

    }
}
</style>