<script>
export default {
    name: "AppSlider"
}
</script>
<template>
    <div class="slider">
        <div class="image-slider">
            <img src="/img/h3-rev-img-6.png" alt="">
        </div>
        <div class="btn prev">
            <span>PREV</span>
        </div>
        <div class="btn next">
            <span>NEXT</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './../styles/variables.scss' as *;

.slider {
    background-image: url("/img/h3-rev-img-5.png");
    height: calc(100% - 80px);
    background-repeat: no-repeat;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;


    .image-slider {
        width: 25%;
    }

    .btn {
        color: $red;
        background-color: $white;
        width: 60px;
        height: 50px;
        border-radius: 50%;
        text-align: center;
        font-size: 0.6rem;
        padding-top: 5px;
        font-weight: 500;
        top: 50%;
        transform: translate(-50%, 0);
    }

    .btn.next {
        position: absolute;
        right: -35px;
        transform: rotate(270deg);

    }

    .btn.prev {
        position: absolute;
        left: -35px;
        transform: rotate(-270deg);
    }
}
</style>