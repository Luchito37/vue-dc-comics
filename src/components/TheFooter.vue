<template>
<div class="bg-dark">
    <div class="container">
    <div class="row d-flex justify-content-between">
        <div class="col">
            <nav class="navbar">
                <form class="container-fluid justify-content-start">
                    <button class="btn btn-outline-primary me-2 text-white myBottom" type="button">Sign-Up NOW!</button>
                </form>
            </nav>
        </div>
        <div class="col d-flex justify-content-end align-items-center">
            <h5 class="text-primary p-2">FOLLOW US</h5>
            <ul class="list-unstyled navSize d-flex">
                <li v-for="footericon in footerLinks" :key="footericon.img">
                    <a class="nav-link text-black p-2" href="#">
                        <img :src="footericon.img" alt="" width="40" height="40" class="d-inline-block align-text-top p-1">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</div>
</div>
</template>

<script>

export default{
    name: "TheFooter",
    data() {
        return {
            footerLinks: [
                {
                    img: "img/footer-facebook.png",
                },
                {
                    img: "img/footer-periscope.png",
                },
                {
                    img: "img/footer-pinterest.png",
                },
                {
                    img: "img/footer-twitter.png",
                },
                {
                    img: "img/footer-youtube.png",
                },

            ]
        }
    }
};
</script>


<style lang="scss" scoped>

@import "../assets/general";

</style>