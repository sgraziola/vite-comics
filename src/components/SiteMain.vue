<script>
import Jumbotron from './Jumbotron.vue'
import CallToAction from './CallToAction.vue';
import ComicsList from './ComicsList.vue';

export default {
    name: "SiteMain",
    components: {
        CallToAction,
        Jumbotron,
        ComicsList
    }
}

</script>
<template>

    <main id="site_main">
        <Jumbotron />

        <ComicsList />

        <CallToAction />
    </main>

</template>

<style lang="scss" scoped>

</style>