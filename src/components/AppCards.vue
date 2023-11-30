<script>
export default {
    props: ["boxes"],
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
<style></style>