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

    <div class="container m_neg">
        <button class="main_btn btn_big shadow mb-4"><a href="#">CURRENT SERIES</a></button>

        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4 row-cols-lg-6 g-5">

            <Comic v-for="Comic in comics" :thumb="Comic.thumb" :title="Comic.series" />

        </div>
        <div class="load text-center">
            <button class="main_btn btn_reg shadow mb-4"><a href="#">LOAD MORE</a></button>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.btn_big {
    font-size: 1.7rem;
}

.btn_reg {
    margin-top: 3rem;
    width: 200px;
    font-size: 14px;
}
</style>