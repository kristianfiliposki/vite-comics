<script>
import AppSocial from '../components/AppSocial.vue'
export default {
    components: { AppSocial },
    data() {
        return {
            FooterTools: [
                {
                    nome: "DC COMICS",
                    options: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Video",
                        "news",
                    ]
                },
                {
                    nome: "DC",
                    options: [
                        "Term of use",
                        "Privacy policy",
                        "Ad joiche",
                        "Ad Advertising",
                        "Jobs",
                        "Subscrition",
                        "Talent Workshop",
                        "CPSP Certificates",
                        "Rating",
                        "Shop helps",
                        "Contact us",

                    ]
                },
                {
                    nome: "SITES",
                    options: [
                        "DC",
                        "Mad Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Powers",

                    ]
                },
                {
                    nome: "SHOP",
                    options: [
                        "Shops",
                        "Shops Dc Colletibles",
                    ]
                },
            ]
        }
    },
    mounted() { },
}
</script>
<template>
    <div class="container">
        <div class="wrapper">
            <div class="option" v-for="tool in FooterTools">
                <div>
                    {{ tool.nome }}
                </div>
                <div v-for="option in tool.options">
                    {{ option }}
                </div>
            </div>
        </div>
    </div>
    <AppSocial />
</template>
<style scoped>
.container {
    width: 100%;
    height: 60vh;
    background-image: url(../img/footer-bg.jpg);
    background-size: cover;
    color: white;
    display: flex;
    align-items: center;
}

.wrapper {
    display: flex;
    flex-wrap: wrap;
    width: 30%;
    margin-left: 10%;
    align-items: flex-start;
}

.option {
    margin: 2px 10px;
}
</style>