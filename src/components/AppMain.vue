<script>
export default {
    props: ["boxes"],
    data() {
        return {
        }
    },
    mounted() { }
}
import boxes from '../App.vue'
</script>
<template>
    <div id="container">
        <div class="WrapperBox">
            <div v-for="element in boxes " class="box">
                {{ element.series }}
                <div class="foto">
                    <img :src="element.thumb" alt="">
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
* {
    box-sizing: border-box;
}

#container {
    background-color: #1c1c1c;
    color: white;
    font-weight: 800;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 0.7em;

}

#container>div {
    font-family: sans-serif;

}

.WrapperBox {
    display: flex;
    width: 75%;
    height: 70%;
    flex-wrap: wrap;
}

.box {
    margin: 2em;
    width: calc((100% / 6) - 2em);
}

.foto {
    width: 100%;
    aspect-ratio: 1;
}

.foto img {
    width: 100%;
    height: 100%;
}
</style>