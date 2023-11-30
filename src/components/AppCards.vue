<script>
export default {
    props: ["box"],
}

</script>
<template >
    <div class="box">
        <div>
            {{ box.series }}
        </div>
        <div class="foto">
            <img :src="box.thumb" alt="">
        </div>
    </div>
</template>
<style>
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