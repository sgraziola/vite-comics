<script>
export default {
    name: "CallToAction",
    data() {
        return {
            calls: [
                {
                    title: "DIGITAL COMICS",
                    image: "buy-comics-digital-comics.png"
                },
                {
                    title: "DC MERCHANDISE",
                    image: "buy-comics-merchandise.png"

                },
                {
                    title: "SUBSCRIPTION",
                    image: "buy-comics-subscriptions.png"

                },
                {
                    title: "COMIC SHOP LOCATOR",
                    image: "buy-comics-shop-locator.png"

                },
                {
                    title: "DC POWER VISA",
                    image: "buy-dc-power-visa.svg"
                },
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }

    }
}
</script>

<template>
    <section class="call_to_action py-5">
        <div class="container">
            <div class="row row-cols-5">
                <div class="col d-flex align-items-center justify-content-evenly" v-for="call in calls">
                    <a href="#" class="d-flex align-items-center">
                        <img class="img-fluid" :src="getImageUrl(call.image)" alt="">
                        <h6>{{ call.title }}</h6>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>

</style>