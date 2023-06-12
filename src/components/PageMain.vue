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
        <!-- sezione slogan -->
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
            <!-- sezione combo special  -->
        </section>
        <section class="special">
            <div class="special-image">
                <img src="/img/h1-img-4.jpg" alt="">
            </div>
            <div class="combo">
                <div class="text-combo">
                    <h2>SPECIALS *</h2>
                    <span class="lorem">Lorem ipsum dolor sit amet consectetur adipisicing elit.Praesent ut</span>
                    <ul>
                        <li>
                            <span class="price">
                                <i class="fa-solid fa-dollar-sign">
                                </i>
                                10
                            </span>
                            <strong>COMBO PICCOLO</strong>
                        </li>
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit.Praesent ut aliquam
                            dui.
                        </li>
                        <li>
                            <span class="price">
                                <i class="fa-solid fa-dollar-sign">
                                </i>
                                20
                            </span>
                            <strong>COMBO MEZZO</strong>
                        </li>
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit.Praesent ut aliquam
                            dui.
                        </li>
                        <li>
                            <span class="price">
                                <i class="fa-solid fa-dollar-sign">
                                </i>
                                30
                            </span>
                            <strong>COMBO GRANDE</strong>
                        </li>
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit.Praesent ut aliquam
                            dui.
                        </li>

                    </ul>
                </div>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="">
                </div>
            </div>
        </section>
        <!-- sezione bg repeat -->
        <section class="bg-repeat">
            <div class="bg top"></div>
            <div class="bg middle">
                <div class="text-middle">
                    GO AHEAD AND BUILD YOUR OWN PIZZA WE WON'T JUDGE!
                </div>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="">
                </div>
            </div>
            <div class="bg bottom"></div>
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


        li {
            margin: 10px 0;
        }

        .price {
            color: $color-price;
            font-weight: 600;

        }

        .lorem {
            font-size: 0.8rem;
            color: grey;

        }

        .list {
            margin-left: 37px;
        }


    }

    .combo {
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
    }

}

.bg-repeat {
    height: 380px;
}

.bg {
    background-size: 85%;
    background-image: url("/img/h3-background-img.jpg");
}

.top {
    height: 100px;
    background-position: bottom 0 left 80px;
}

.middle {
    height: 180px;
    background-position: top 0 left 80px;
    position: relative;

    .text-middle {
        width: 25%;
        text-align: left;
        font-size: 2rem;
        font-weight: 600;
        color: $white;
        position: absolute;
        top: -5%;
        left: 20%;
    }
}

.bottom {
    height: 100px;
    background-position: top 70% left 80px;
}
</style>