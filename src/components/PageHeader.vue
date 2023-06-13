<script>
import AppSlider from './AppSlider.vue';
export default {
    name: "PageHeader",
    components: {
        AppSlider,
    },
    props: {
        details: Array
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
                    <li v-for="link in details">
                        {{ link.text }}
                    </li>
                </ul>
            </nav>
            <div class="shop">
                <ul>
                    <li class="pay">
                        <img src="/svg/svg-1.svg" alt="">
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
        font-size: 0.8rem;
    }

    ul {
        display: flex;
        gap: 10px;
        align-items: center;

        .logo {
            width: 80px;
        }
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