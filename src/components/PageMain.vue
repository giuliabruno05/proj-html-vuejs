<script>
export default {
    name: "PageMain"
}
</script>

<template>
    <main>
        <div class="container">
            <div class="image">
                <img src="/img/h3-img-1.jpg" alt="">
            </div>
            <div class="image">
                <img src="/img/h3-img-2.jpg" alt="">
            </div>
            <div class="image">
                <img src="/img/h3-img-3.jpg" alt="">
            </div>
            <div class="image">
                <img src="/img/h3-img-4.jpg" alt="">
            </div>
        </div>
        <section class="slogan">
            <div class="btn prev">
                <span>PREV</span>
            </div>
            <div class="btn next">
                <span>NEXT</span>
            </div>
            <div class="text">
                <i class="fa-solid fa-quote-left"></i><br>
                <span>"FORGET THE TRENDY PIZZA SHPOS,THIS HIDDEN SPORT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"
                </span><br>
                <span class="post">WASHINGTON POST 2018</span>
            </div>
            <div class="icon-pizza">
                <img src="/svg/svg-4.svg" alt="">
            </div>
        </section>
        <section class="special">
            <div class="special-image">
                <img src="/img/h1-img-4.jpg" alt="">
            </div>
            <div class="combo">
                <div class="text-combo">
                    <h3>SPECIALS *</h3>
                    <span class="lorem">Lorem ipsum dolor sit amet consectetur adipisicing elit.Praesent ut</span>
                    <span></span>
                </div>
            </div>
        </section>
    </main>
</template>
<style lang="scss" scoped>
@use './../styles/variables.scss' as *;

.container {
    display: flex;
    width: 100%;
    gap: 5px;
    padding-top: 5px;

}

.slogan {
    height: 300px;
    background-image: url("/img/h3-testimonials-bckgrnd.jpg");
    background-size: 100%;
    text-align: center;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;

    i {
        color: $third-color;
        font-size: 2rem;
    }

    .text {
        width: 55%;

        .post {
            color: $red;
            margin: 10px 0;
            font-size: 0.6rem;
        }
    }
}

.special {
    display: flex;
    width: 100%;

    .special-image {
        width: 50%;
    }

    .text-combo {
        width: 60%;

        .lorem {
            font-size: 0.8rem;
            color: grey;
        }
    }

    .combo {
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}
</style>