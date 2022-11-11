<script>
export default {
    name: 'Comic',
    props: {
        thumb: String,
        title: String,
    }
}
</script>

<template>
    <div class="col">
        <div class="comic">
            <img :src="thumb" :alt="title">
            <h6>{{ title }}</h6>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.comic {
    h6 {
        text-transform: uppercase;
    }
}
</style>