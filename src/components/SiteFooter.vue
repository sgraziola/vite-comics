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
                    title: "Shop",
                    list: ["Shop DC", "Shop DC Collectibles"],
                },
                {
                    title: "DC",
                    list: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                },
                {
                    title: "Sites",
                    list: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
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
                <div class="row gx-5">
                    <div class="col" v-for="link in menuLinks">
                        <h4>{{ link.title }}</h4>
                        <ul class="list-unstyled">
                            <li v-for="item in link.list"><a href="#">{{ item }}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer_bot py-4">
            <div class="container d-flex justify-content-between">
                <div class="signup">
                    <a href="#" class="btn text-white border border-2 border-primary">SIGN-UP NOW!</a>
                </div>
                <div class="socials d-flex justify-content-around">
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>

                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>

</style>