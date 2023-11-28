<script>
export default {
    data() {
        return {
            cards: [
                {
                    nome: "Digital Comics",
                    foto: "/src/img/buy-comics-digital-comics.png",
                },
                {
                    nome: "Dc Merchandise",
                    foto: "/src/img/buy-comics-merchandise.png",
                },
                {
                    nome: "Subscription",
                    foto: "/src/img/buy-comics-subscriptions.png",
                },
                {
                    nome: "Comic Shop Locator",
                    foto: "/src/img/buy-comics-shop-locator.png",
                },
                {
                    nome: "Dc Power Visa",
                    foto: "/src/img/buy-dc-power-visa.svg",
                },



            ]
        }
    },
    mounted() { },
}
</script>
<template>
    <div id="container">
        <div class="wrapper">
            <div v-for="card, index in cards" class=box>
                <div class="foto">
                    <img :src=card.foto alt="porcod..">
                </div>
                <div>
                    {{ card.nome }}
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
#container {
    height: 20vh;
    background-color: rgba(2, 130, 249, 255);
    color: white;
    font-weight: 800;
    display: flex;
    justify-content: center;
    width: 100%;
}

#container div {
    font-family: sans-serif;
}

.wrapper {
    width: 80%;
    display: flex;

}

.box {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-right: 2em;
}

.foto {
    width: 30%;
    height: 30%;
    margin-right: 1em;
}

img {
    width: 100%;
    height: 100%;

}
</style>