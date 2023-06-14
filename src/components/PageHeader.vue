<script>
import AppSlider from './AppSlider.vue';
export default {
    name: "PageHeader",
    components: {
        AppSlider,
    },
    props: {
        details: Array,
        element: Array
    }
}
</script>

<template>
    <header>
        <div class="row">
            <div>
                <button class="button"> ORDER ONLINE</button>
            </div>
            <!-- nav header  -->
            <nav>
                <ul>
                    <li class="mustache">
                        <img src="/svg/svg-2.svg" alt="img baffi">
                    </li>
                    <li v-for="link in details">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                    <li>
                        <div class="logo">
                            <img src="/img/h5-logo-divided-header.png" alt="logo">
                        </div>
                    </li>
                    <li v-for="menu in element">
                        <a :href="menu.url">{{ menu.text }}</a>
                    </li>
                </ul>

            </nav>
            <div class="shop">
                <ul>
                    <li class="pay">
                        <img src="/svg/svg-1.svg" alt="icon scooter">
                        CART
                    </li>
                    <li>
                        <i class="fa-solid fa-magnifying-glass fa-rotate-90"></i>
                        SEARCH
                    </li>
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
        font-size: 0.7rem;


    }

    ul {
        display: flex;
        gap: 15px;
        align-items: center;

        li:hover {
            cursor: pointer;
            transform: scale(1.2);
        }

        .logo {
            width: 80px;

        }
    }

    .mustache {
        width: 15px;
        height: 15px;
        fill: $white;

    }

    .pay {
        display: flex;
        align-items: center;
        gap: 5px;
    }

    .pay img {
        width: 30px;

    }
}
</style>