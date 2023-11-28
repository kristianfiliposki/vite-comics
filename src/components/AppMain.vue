<script>
export default {
    data() {
        return {
            contenuto: "--> Content goes here <-- ",
        }
    },
    mounted() { }
}
</script>
<template>
    <div id="container">
        <div>
            {{ contenuto }}
        </div>
    </div>
</template>
<style scoped>
#container {
    height: 15vh;
    background-color: #1c1c1c;
    color: white;
    font-weight: 800;
    display: flex;
    justify-content: center;
    align-items: center;
}

#container div {
    font-family: sans-serif;
    width: 80%;

}
</style>