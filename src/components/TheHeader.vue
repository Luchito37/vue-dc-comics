<template>
    <div class="container">
        <div class="row">
                <div class="col">
                <nav class="navbar">
                    <div class="container-fluid">
                        <a class="navbar-brand" href="#">
                            <img src="../assets/img/dc-logo.png" alt="" width="100" height="100" class="d-inline-block align-text-top">
                        </a>
                        <div>
                            <ul class="nav navSize">
                                <li class="nav-item " v-for="link in navLinks" :key="link">
                                    <a class="nav-link myLink" :href="link.href">{{link.name}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </nav>
            </div>
        </div>
    </div>
</template>

<script>

export default{
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    name: "CHARACTERS",
                    href: "#"
                },
                {
                    name: "COMICS",
                    href: "#"
                },
                {
                    name: "MOVIES",
                    href: "#"
                },
                {
                    name: "TV",
                    href: "#"
                },
                {
                    name: "GAMES",
                    href: "#"
                },
                {
                    name: "COLLECTIBLES",
                    href: "#"
                },
                {
                    name: "VIDEOS",
                    href: "#"
                },
                {
                    name: "CHARACTERS",
                    href: "#"
                },
                {
                    name: "NEWS",
                    href: "#"
                },
                {
                    name: "SHOP",
                    href: "#"
                },

            ]
        }
    }
};
</script>


<style lang="scss" scoped>

@import "../assets/general";

.navSize{
    font-size: 12px;
}

</style>
