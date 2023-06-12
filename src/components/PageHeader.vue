<script>
import AppSlider from './AppSlider.vue';
export default {
    name: "PageHeader",
    components: {
        AppSlider,
    }
}
</script>

<template>
    <header>
        <div class="row">
            <div>
                <button class="button"> ORDER ONLINE</button>
            </div>
            <nav>
                <ul>
                    <li>HOME</li>
                    <li>PAGES</li>
                    <li>MENU</li>
                    <li>
                        <div class="logo">
                            <img src="/img/h5-logo-divided-header.png" alt="">
                        </div>
                    </li>
                    <li>EVENT</li>
                    <li>BLOG</li>
                    <li>LANDING</li>
                </ul>
            </nav>
            <div class="shop">
                <ul>
                    <li>CART</li>
                    <li>SEARCH</li>
                </ul>
            </div>
        </div>
        <AppSlider />
    </header>
</template>
<style lang="scss" scoped>
@use './../styles/variables.scss' as *;

header {
    background-image: url("/img/cielostellato.PNG");
    height: 550px;
    background-position: bottom;
    position: relative;

    .row {
        display: flex;
        color: $white;
        justify-content: space-around;
        align-items: center;
        padding: 10px;
        height: 80px;
        font-size: 0.8rem;
    }



    .button {
        margin-right: 10px;
        padding: 15px;
        background-color: #d2401e;
        border: hidden;
        color: $white;
    }

    ul {
        display: flex;
        gap: 10px;
        align-items: center;

        .logo {
            width: 80px;
        }
    }
}
</style>