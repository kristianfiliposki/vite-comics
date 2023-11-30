<script>
export default {
    name: "AppHeader",
    data() {
        return {
            tools: ["characters", "comics", " movies", " tv", "games", "collectibles", "video", " fans", " news", " shop",]
        }
    },
    mounted() {
        console.log("Componente Header caricato");
    }
}
</script>
<template>
    <section>
        <div class="container">
            <div class="foto"><img src="../img/dc-logo.png" alt=""></div>

            <div id="box-tools">
                <div v-for="tool in tools">{{ tool }}</div>
            </div>
        </div>
    </section>
</template>
<style scoped>
section {
    width: 100%;
    height: 10vh;
    display: flex;
    justify-content: center;

}

.container {
    display: flex;
    justify-content: space-between;
    width: 80%;
}

.foto {
    height: 80%;
    display: flex;
    align-items: center;
}

.foto img {
    padding-top: 22px;
    width: 20%;

}

#box-tools {
    display: flex;
    align-items: center;

}

#box-tools div {
    margin: 3px;
    font-size: 1.2em;
}

#box-tools div:hover {
    border-bottom: 2px solid blue;
    color: blue;

}
</style>