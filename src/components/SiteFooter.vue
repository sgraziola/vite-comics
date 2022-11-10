<script>
export default {
    name: "SiteFooter",
    data() {
        return {
            menuLinks: [
                {
                    title: "Dc Comics",
                    list: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
                },
                {
                    title: "DC",
                    list: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                },
                {
                    title: "Sites",
                    list: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
                },
                {
                    title: "Shop",
                    list: ["Shop DC", "Shop DC Collectibles"],
                },
            ]
        }
    }
}

</script>
<template>

    <footer id="site_footer">
        <div class="footer_top">
            <div class="container py-4 d-flex justify-content-between">
                <div class="row row-cols-3">
                    <div class="col" v-for="link in menuLinks">
                        <h4>{{ link.title }}</h4>
                        <ul class="list-unstyled">
                            <li v-for="item in link.list">{{ item }}</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>
.footer_top {
    color: white;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        background-image: url("../assets/img/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position: right;
    }

    h4 {
        text-transform: uppercase;
    }

    li {
        color: gray;
    }
}
</style>