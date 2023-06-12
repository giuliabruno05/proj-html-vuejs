<script>
export default {
    name: "PageFooter"
}
</script>

<template>
    <footer>
        <div class="location">
            <img class="logo-footer" src="/img/footer-bottom-img.png" alt="">
        </div>
        <div class="footer-img">
            <div class="icon-pizza">
                <img src="/svg/svg-4.svg" alt="">
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@use './../styles/variables.scss' as *;

footer {
    display: flex;
    width: 100%;
    height: 400px;

    .location {
        background-image: url("/img/cielostellato.PNG");
        background-position: bottom;
        width: 50%;
        height: 100%;
        position: relative;

        .logo-footer {
            width: 80px;
            position: absolute;
            bottom: 10px;
            right: 10px;

        }

    }

    .footer-img {
        background-image: url("/img/footer-img-1.jpg");
        width: 50%;
        background-position: center;
        background-size: cover;
        height: 100%;
        position: relative;

    }
}
</style>