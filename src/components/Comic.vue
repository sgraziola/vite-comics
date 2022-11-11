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
            <span>{{ title }}</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>