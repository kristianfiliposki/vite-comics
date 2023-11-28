<script></script>
<template>
    <div class="last">
        <div class="signUp">Sign-up</div>
        <div class="social">
            <div class="follow">Follow us</div>
            <div>
                <img src="../img/footer-facebook.png" alt="">
                <img src="../img/footer-periscope.png" alt="">
                <img src="../img/footer-pinterest.png" alt="">
                <img src="../img/footer-twitter.png" alt="">
                <img src="../img/footer-youtube.png" alt="">
            </div>
        </div>
    </div>
</template>
<style scoped>
.last {
    display: flex;
    height: 10vh;
    background-color: black;
    align-items: center;
    justify-content: space-around;
    color: white;
}

.signUp {
    border: 3px solid blue;
    padding: 1em;
    font-size: 1.3em;
}

.follow {
    color: blue;
    font-size: 1.2em;
    font-weight: 900;
    margin-right: 12px;
}

.social {
    display: flex;
    justify-content: space-around;
    align-items: center;
}

img {
    margin: 6px;
}
</style>