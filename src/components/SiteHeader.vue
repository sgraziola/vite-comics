<script>
export default {
    name: "SiteHeader",
    data() {
        return {
            navLinks: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'Tv',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                },

            ]
        }
    }
}

</script>
<template>

    <header id="site_header">
        <div class="container">
            <nav class="navbar navbar-expand-lg py-4">
                <div class="container-fluid">
                    <a class="navbar-brand" href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
                    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="collapse navbar-collapse" id="navbarNav">
                        <ul class="navbar-nav ms-auto">
                            <li class="nav-item" v-for="link in navLinks">
                                <a class="nav-link" :class="link.text === 'Comics' ? 'selected' : ''" :href="link.href">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </div>
    </header>

</template>

<style lang="scss" scoped>

</style>