<script>
export default {
    name: "PageMain",
    data() {
        return {
            pathImage: [
                "/img/h3-img-1.jpg",
                "/img/h3-img-2.jpg",
                "/img/h3-img-3.jpg",
                "/img/h3-img-4.jpg"
            ],
            imageClient: [
                "/img/h1-team-1a-700x700.jpg",
                "/img/h1-team-2a.jpg",
                "/img/h1-team-4a.jpg",
                "/img/h1-team-3a.jpg"
            ],
            pathPizza: [
                {
                    path: "/img/h3-product-img-1a-100x100.png",
                    name: "BISMARCK",
                    sale: "$35.00",
                    price: "$30.00"
                },
                {
                    path: "/img/h3-product-img-2a-150x150.png",
                    name: "FIORI DI ZUCCA",
                    sale: "",
                    price: " $7.00 - $50.00"
                },
                {
                    path: "/img/h3-product-img-3a-150x150.png",
                    name: "VALDOSTANA",
                    sale: "",
                    price: "$55.00"
                },
                {
                    path: "/img/h3-product-img-4a-150x150.png",
                    name: "PIZZA TARTUFATA",
                    sale: "",
                    price: "$45.00"
                }, {
                    path: "/img/h3-product-img-5a-150x150.png",
                    name: "FRANCESCANA",
                    sale: "",
                    price: "$25.00"
                },
                {
                    path: "/img/h3-product-img-6a-100x100.png",
                    name: "CAMPAGNOLA",
                    sale: "",
                    price: "$50.00 - $95.00"
                }


            ]
        }
    }
}
</script>

<template>
    <main>
        <div class="container">
            <div class="image" v-for="path in pathImage">
                <img :src="path" alt="">
            </div>
        </div>
        <!-- sezione slogan -->
        <section id="slogan">
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
        <!-- sezione combo special -->
        <section id="special">
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
        <section id="bg-repeat">
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
        <!-- sezione team -->
        <section id="team">
            <div class="container">
                <div class="team" v-for="path in imageClient">
                    <img :src="path" alt="">
                </div>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="">
                </div>
            </div>
        </section>
        <!-- sezione clienti -->
        <section id="clienti">
            <div class="container">
                <div class="logo-clienti">
                    <img src="/img/h1-clients-img-4.png" alt="client logo">
                </div>
                <div class="logo-clienti">
                    <img src="/img/h1-clients-img-3.png" alt="client logo">
                </div>
                <div class="logo-clienti">
                    <img src="/img/h1-clients-img-1.png" alt="client logo">
                </div>
                <div class="logo-clienti">
                    <img src="/img/h1-clients-img-2.png" alt="client logo">
                </div>
                <div class="logo-clienti">
                    <img src="/img/h1-clients-img-5.png" alt="client logo">
                </div>
            </div>
        </section>
        <!-- sezione scegli la pizza -->
        <section id="choosePizza">
            <div class="text-choosePizza">
                <h6>CHOOSE YOUR FLAVOR</h6>
                <h3>THE BEST PIZZA IN TOWN</h3>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit.Ut blandit arcu in pretium
                    molestie.Interdum et malesuada fames ac.
                </span>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="">
                </div>
            </div>
            <div class="container">

                <div class="pizza" v-for="element in pathPizza">
                    <img :src="element.path" alt="">
                    <h4>{{ element.name }}</h4>
                    <span class="sale" v-if="element.sale !== ''">{{ element.sale }}</span>
                    <span class="price">{{ element.price }}</span>
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

#slogan {
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

#special {
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

#bg-repeat {
    height: 380px;

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
}



#team {
    .container {
        position: relative;
        gap: 0;

        .team {
            height: 300px;
            width: 100%;

        }
    }
}


#clienti {
    height: 200px;
    background-color: #f7f7f2;

    .container {
        height: 100%;
        align-items: center;
        width: 70%;
        margin: 0 auto;



    }
}

#choosePizza {
    height: 400px;
    padding: 20px;


    .text-choosePizza {
        text-align: center;
        margin: 20px 0;
        position: relative;

        span {
            width: 40%;
            margin: 0 auto;
        }

        .icon-pizza {
            background-color: #f7f7f2;
        }


        h6 {
            color: $price;
            margin-bottom: 10px;
        }

        span {
            font-size: 0.8rem;
            color: grey;
            margin-top: 10px;
            display: inline-block;
        }
    }

    .pizza {
        width: 150px;
        font-size: 0.7rem;
        text-align: center;
        color: $third-color;
        margin-top: 20px;

        h4 {
            margin-top: 10px;
            margin-bottom: 5px;
        }

        .price {
            color: $price;
            font-weight: 600;
            margin: 0 10px;
        }

        .sale {
            text-decoration: line-through;
        }

    }

    .container {
        justify-content: space-between;

    }
}
</style>