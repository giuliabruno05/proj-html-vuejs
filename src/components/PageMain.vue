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
                {
                    path: "/img/h1-team-1a-700x700.jpg",
                    name: "JHONNY FRANKLIN",
                    role: "Chef"
                },
                {
                    path: "/img/h1-team-2a.jpg",
                    name: "ABBY FRANKLIN",
                    role: "Kitchen Porter"
                },
                {
                    path: "/img/h1-team-4a.jpg",
                    name: "LEWIS FRANKLIN",
                    role: "Sous Chef"
                },
                {
                    path: "/img/h1-team-3a.jpg",
                    name: "JULIE FRANKLIN",
                    role: "Manager"
                },

            ],
            pathPizza: [
                {
                    path: "/img/h3-product-img-1a-100x100.png",
                    name: "BISMARCK",
                    sale: "$35.00",
                    price: "$30.00",
                    soldOut: false
                },
                {
                    path: "/img/h3-product-img-2a-150x150.png",
                    name: "FIORI DI ZUCCA",
                    sale: "",
                    price: " $7.00 - $50.00",
                    soldOut: false
                },
                {
                    path: "/img/h3-product-img-3a-150x150.png",
                    name: "VALDOSTANA",
                    sale: "",
                    price: "$55.00",
                    soldOut: true
                },
                {
                    path: "/img/h3-product-img-4a-150x150.png",
                    name: "PIZZA TARTUFATA",
                    sale: "",
                    price: "$45.00",
                    soldOut: false
                }, {
                    path: "/img/h3-product-img-5a-150x150.png",
                    name: "FRANCESCANA",
                    sale: "",
                    price: "$25.00",
                    soldOut: false
                },
                {
                    path: "/img/h3-product-img-6a-100x100.png",
                    name: "CAMPAGNOLA",
                    sale: "",
                    price: "$50.00 - $95.00",
                    soldOut: false
                }


            ]
        }
    }
}
</script>

<template>
    <main>
        <!-- sezione sponsor -->
        <section id="sponsor">
            <div class="container">
                <div class="image" v-for="path in pathImage">
                    <img :src="path" alt="sponsor">
                    <div class="image-hover">
                        <div class="label">
                            <i class="fa-regular fa-eye"></i>
                        </div>
                    </div>
                </div>
            </div>
        </section>
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
                <img src="/svg/svg-4.svg" alt="icon pizza">
            </div>
            <!-- sezione combo special  -->
        </section>
        <!-- sezione combo special -->
        <section id="special">
            <div class="special-image">
                <img src="/img/h1-img-4.jpg" alt="foto special">
                <img class="foto-special" src="/img/h1-img-7n.png" alt="pizza special">
            </div>
            <div class="combo">
                <div class="text-combo">
                    <h2>SPECIALS *</h2>
                    <span class="lorem">Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesent ut</span>
                    <ul>
                        <li>
                            <span class="price">
                                <i class="fa-solid fa-dollar-sign">
                                </i>
                                10
                            </span>
                            <strong>COMBO PICCOLO</strong>
                        </li>
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesent ut aliquam
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
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesent ut aliquam
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
                        <li class="lorem list">Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesent ut aliquam
                            dui.
                        </li>

                    </ul>
                </div>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="icon pizza">
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
                    <img src="/svg/svg-4.svg" alt="icon pizza">
                </div>
            </div>
            <div class="bg bottom"></div>
        </section>
        <!-- sezione team -->
        <section id="team">
            <div class="container">
                <div class="team" v-for="team in imageClient">
                    <img :src="team.path" alt="foto team">
                    <div class="image-hover-team">
                        <div class="contacts">
                            <div>
                                <h5>{{ team.name }}</h5>
                                <span>{{ team.role }}</span>
                                <div class="icon">
                                    <a href="#">
                                        <i class="fa-brands fa-instagram"></i>
                                    </a>
                                    <a href="#">
                                        <i class="fa-brands fa-twitter"></i>
                                    </a>
                                    <a href="#">
                                        <i class="fa-brands fa-facebook-f"></i>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
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
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut blandit arcu in pretium molestie.Interdum
                    et malesuada fames ac.
                </span>
                <div class="icon-pizza">
                    <img src="/svg/svg-4.svg" alt="icon pizza">
                </div>
            </div>
            <div class="container">
                <div class="pizza" v-for="element in pathPizza">
                    <img :src="element.path" alt="foto pizza">
                    <h4>{{ element.name }}</h4>
                    <span class="sale" v-if="element.sale !== ''">{{ element.sale }}</span>
                    <span class="price">{{ element.price }}</span>
                    <div class="soldOut label" v-if="element.soldOut">
                        SOLD
                    </div>
                </div>
            </div>
            <div class="icon-cicle">
                <img src="/svg/svg-10.svg" alt="icon svg">
            </div>
        </section>
        <!-- sezioni eventi -->
        <section id="events">
            <div class="text-event">
                <div class="date-event">
                    <h6>MADE WITH LOVE</h6>
                    <h3>DELISH PIZZA DEALS</h3>
                    <ul>
                        <li class="dashed">
                            <div class="data">
                                <span class="number">
                                    02
                                </span><br>
                                <span>NOV</span>
                            </div>
                            <div class="text">
                                TRADITIONAL NEAOPOLITAN PIES IN KYOTO PIZZA MERCATO
                                <div class="event-location">
                                    <i class="fa-solid fa-location-dot"></i>
                                    204 E.piazzetta tommaso
                                </div>
                            </div>
                        </li>
                        <li class="dashed">
                            <div class="data">
                                <span class="number">
                                    03
                                </span><br>
                                <span>NOV</span>
                            </div>
                            <div class="text">
                                TERRAZZA PATIO DINING SPACE OPENING THIS WEEKEND
                                <div class="event-location">
                                    <i class="fa-solid fa-location-dot"></i>
                                    204 E.piazzetta tommaso
                                </div>
                            </div>
                        </li>
                        <li>
                            <div class="data">
                                <span class="number">
                                    05
                                </span><br>
                                <span>NOV</span>
                            </div>
                            <div class="text">
                                SIENNA PRIVATE DINING ROOM WITH STHEPANE BRUNN
                                <div class="event-location">
                                    <i class="fa-solid fa-location-dot"></i>
                                    204 E.piazzetta tommaso
                                </div>
                            </div>
                        </li>
                    </ul>

                </div>
                <div class="image-event">
                    <div class="icon-pizza">
                        <img src="/svg/svg-4.svg" alt="icon pizza">
                    </div>
                    <div class="shop">
                        <img src="/svg/svg-9.svg" alt="shop">
                    </div>
                </div>
            </div>

        </section>
        <!-- sezione pre-order table -->
        <section id="preOrder">
            <div class="form">
                <input type="text" placeholder="1 person ">
                <span>FOR</span>
                <input type="date">
                <span>AT</span>
                <input type="datetime" placeholder="7:00 pm">
                <button class="button">BOOK A TABLE</button>
                <span class="sponsor">*Powered by open table</span>
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

#sponsor {
    .container {
        min-height: 100px;

        .image {
            width: calc(100% / 4 - 5px);


            &:hover img {
                display: none;
            }

            &:hover .image-hover {
                display: block;
            }
        }

        .image-hover {
            background-image: url("/img/pois.jpg");
            position: relative;
            width: 100%;
            height: 100%;
            display: none;

            .label {
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
        }

    }


}


#slogan {
    height: 300px;
    background-image: url("/img/h3-testimonials-bckgrnd.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
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

    .icon-pizza {
        background-color: #f7f7f2;
    }
}

#special {
    display: flex;
    width: 100%;

    .special-image {
        width: 50%;
        position: relative;

        .foto-special {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 35%;
            transform: translate(-50%, -50%);

        }
    }

    .text-combo {
        width: 60%;


        li {
            margin: 15px 0;


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

    .icon-pizza {
        background-color: #f7f7f2;
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
        min-height: 100px;

        .team {
            width: 100%;

            &:hover img {
                display: none;
            }

            &:hover .image-hover-team {
                display: block;
            }
        }

        .image-hover-team {
            background-image: url("/img/pois.jpg");
            width: 100%;
            height: 100%;
            position: relative;
            display: none;



            .contacts {
                width: 90%;
                height: 90%;
                background-color: $price;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                display: flex;
                justify-content: center;
                align-items: center;
                color: $white;
                text-align: center;

                span {
                    margin: 10px 0;
                    display: inline-block;
                    font-size: 0.7rem;
                }

            }
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
    padding-top: 30px;
    padding-bottom: 60px;
    position: relative;

    .icon-cicle {

        background-color: #ee2852;
        width: 20px;
        position: absolute;
        bottom: 0;
        right: 0;
        height: 20px;
        text-align: center;

        img {
            width: 10px;
            height: 15px;
            margin-top: 3px;
        }

    }

    .text-choosePizza {
        text-align: center;
        margin: 20px 0;
        position: relative;

        span {
            width: 35%;
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

    .container {
        justify-content: space-between;

        .pizza {
            width: 150px;
            font-size: 0.7rem;
            text-align: center;
            color: $third-color;
            margin-top: 20px;
            position: relative;

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

            .soldOut {
                top: 0;
                right: 0;
            }

        }
    }

}

#events {
    height: 550px;


    .text-event {
        height: 100%;
        display: flex;

        .date-event {
            background-image: url("/img/cielostellato.PNG");
            background-position: bottom;
            height: 85%;
            width: 50%;
            color: $white;
            padding: 60px;

            h6 {
                color: $price;
                font-size: 0.5rem;
                font-weight: normal;
                margin-bottom: 5px;
            }

            h3 {
                margin-bottom: 20px;
                font-weight: 400;
            }

            li {
                margin: 30px 0;
                display: flex;
                justify-content: space-between;
                padding-bottom: 30px;
                width: 90%;

                .text {
                    font-size: 0.9rem;
                    width: 80%;
                }

                .number {
                    font-size: 2rem;
                    font-weight: 600;
                    color: $price;
                    margin-top: -4px;
                    display: inline-block;
                }
            }

            .dashed {
                border-bottom: 1px dashed $third-color;
            }

            span i {
                color: $price;
                font-size: 2rem;
                margin: 10px 0;
            }

            .event-location {
                color: $price;
                font-size: 0.6rem;
                margin: 5px 0;
            }
        }

        .image-event {
            background-image: url("/img/h3-img-5a.jpg");
            width: 50%;
            height: 100%;
            background-size: cover;
            position: relative;

            .shop {
                width: 20px;
                background-color: #fff;
                position: absolute;
                top: 0;
                right: 0;
                height: 20px;
                text-align: center;

                img {
                    width: 10px;
                    height: 15px;
                    margin-top: 3px;
                }

            }
        }
    }
}

#preOrder {
    background-image: url("/img/h3-background-img-3.jpg");
    height: 200px;
    background-size: cover;
    background-position: right;
    margin: 5px 0;
    display: flex;
    justify-content: center;
    align-items: center;



    .form {
        padding: 0 30px;
        width: 10;
        position: relative;


        input {
            border: 1px solid black;
            background-color: #fff;
            padding: 10px;
            margin-right: 30px;
        }

        span {
            color: $white;
            margin-right: 15px;
            display: inline-block;
        }

        .button {
            padding: 12px;
            font-size: 0.7rem;
            min-width: 162px;
        }
    }

    .sponsor {
        font-size: 0.6rem;
        position: absolute;
        bottom: -15px;
        left: 30px;
    }


}
</style>