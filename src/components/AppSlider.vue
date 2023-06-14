<script>
export default {
    name: "AppSlider"
}
</script>
<template>
    <div class="slider">
        <div class="image-slider">
            <img src="/img/h3-rev-img-6.png" alt="img prodotto slider">
        </div>
    </div>
    <div class="btn prev">
        <span>PREV</span>
    </div>
    <div class="btn next">
        <span>NEXT</span>
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


}
</style>