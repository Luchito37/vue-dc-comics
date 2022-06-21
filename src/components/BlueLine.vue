<template>
    <div class="bg-primary py-5">
        <div class="container px-4">
            <div class="row">
                <div class="col">
                        <nav class="navbar">
                            <div class="container-fluid">
                                <a class="navbar-brand d-flex align-items-center text-white iconSize" href="#" v-for="icon in iconLinks" :key="icon">
                                    <img :src="require('../assets/img/buy-comics-digital-comics.png')" alt="" width="80" height="90" class="d-inline-block align-text-top p-3">
                                    {{icon.name}}
                                </a>
                            </div>
                        </nav>
                </div>
            </div>
        </div>
    </div>
</template>


<script>

export default{
    name: "BlueLine",
    data() {
        return {
            iconLinks: [
                {
                    img: "buy-comics-digital-comics.png",
                    name: "DIGITAL COMICS",
                },
                {
                    img: "buy-comics-merchandise.png",
                    name: "DC MERCHANDISE",
                },
                {
                    img: "buy-comics-subscriptions.png",
                    name: "SUBSCRIPTION",
                },
                {
                    img: "buy-comics-shop-locator.png",
                    name: "COMIC SHOP LOCATOR",
                },
                {
                    img: "buy-dc-power-visa.svg",
                    name: "DC POWER VISA",
                },

            ]
        }
    }
};
</script>


<style scoped>

.iconSize{
    font-size: 12px;
}

</style>
