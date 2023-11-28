<script>
export default {
    name: "header",
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
}

.foto img {
    height: 100%;
    width: 100%;

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
    border-bottom: 2px solid #1c1c1c;
    color: #1c1c1c;
    padding-bottom: 2em;

}
</style>