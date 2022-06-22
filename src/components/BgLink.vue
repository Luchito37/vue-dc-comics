<template>
    <div class="jumboDC overflow-hidden">
        <div class="container">
            <div class="row">
                <div class="col-6 d-flex flex-raw my-5 text-white flex-wrap">
                        <div class="px-4">
                            <h3>DC COMICS</h3>
                            <ul class="list-unstyled navSize">
                                <li class=" " v-for="comics in dcComicsLink" :key="comics">
                                    <a class="nav-link text-secondary" href="#">{{comics}}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="px-4">
                            <h3>DC</h3>
                            <ul class="list-unstyled navSize">
                                <li class="nav-item " v-for="linkdc in dcLink" :key="linkdc">
                                    <a class="nav-link text-secondary" href="#">{{linkdc}}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="px-4">
                            <h3>SITES</h3>
                            <ul class="list-unstyled navSize">
                                <li class="nav-item " v-for="site in siteLink" :key="site">
                                    <a class="nav-link text-secondary" href="#">{{site}}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="px-4">
                            <h3>SHOP</h3>
                            <ul class="list-unstyled navSize">
                                <li class="nav-item " v-for="shop in shopLinks" :key="shop">
                                    <a class="nav-link text-secondary" href="#">{{shop}}</a>
                                </li>
                            </ul>
                        </div>
                </div>
                <div class="col-1"></div>
                <div class="col overflow-hidden">
                    <div class="logoDC">
                        <img class="logoDC overflow-auto" src="../assets/img/dc-logo-bg.png" alt="">
                    </div>
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
            dcComicsLink: [
                "Characters",
                "Comics",
                "Marvel",
                "Games",
                "Videse",
                "News",
                "Tv"
            ],

            shopLinks: [
                "Shop DC",
                "Shop DC Collectibles"
            ],

            dcLink: [
                "Characters",
                "Comics",
                "Marvel",
                "Games",
                "Videse",
                "News",
                "Tv",
                "Marvel",
                "Games",
                "Videse",
                "News",
                "Tv"
            ],

            siteLink: [
                "Characters",
                "Comics",
                "Marvel",
                "Games",
                "Videse",
                "News",
                
            ],
        }
    }
};
</script>


<style scoped>

.jumboDC{
    background-image: url(http://localhost:8080/img/footer-bg.1b706117.jpg);
    background-attachment: fixed;
    background-position: center;
    background-size: cover;
}
.logoDC{
    width: 500px;
}

</style>