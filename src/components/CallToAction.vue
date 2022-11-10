<script>
export default {
    name: "CallToAction",
    data() {
        return {
            calls: [
                {
                    title: "DIGITAL COMICS",
                    image: "./src/assets/img/buy-comics-digital-comics.png"
                },
                {
                    title: "DC MERCHANDISE",
                    image: "./src/assets/img/buy-comics-merchandise.png"

                },
                {
                    title: "SUBSCRIPTION",
                    image: "./src/assets/img/buy-comics-subscriptions.png"

                },
                {
                    title: "COMIC SHOP LOCATOR",
                    image: "./src/assets/img/buy-comics-shop-locator.png"

                },
                {
                    title: "DC POWER VISA",
                    image: "./src/assets/img/buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<template>
    <section class="call_to_action py-5">
        <div class="container">
            <div class="row row-cols-5">
                <div class="col d-flex align-items-center justify-content-evenly" v-for="call in calls">
                    <img class="img-fluid" :src="call.image" alt="">
                    <h6>{{ call.title }}</h6>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">

</style>