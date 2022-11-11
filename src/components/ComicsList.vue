<script>
import Comic from './Comic.vue'
import comics from '../data/comics.js'
export default {
    name: "ComicList",
    components: {
        Comic,
    },
    data() {
        return {
            comics,
        }
    }
}
</script>

<template>

    <div class="container">
        <button class="main_btn shadow mb-4"><a href="#">CURRENT SERIES</a></button>

        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4 row-cols-lg-6 g-5">

            <Comic v-for="Comic in comics" :thumb="Comic.thumb" :title="Comic.series" />

        </div>
    </div>

</template>

<style lang="scss" scoped>

</style>