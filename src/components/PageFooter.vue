<script>
export default {
    name: "PageFooter",
    data() {
        return {
            location: [
                {
                    address: "1614 E.Bell Rd #104",
                    city: "Salerno,AZ 85022",
                    number: "(602)867-1010"
                },
                {
                    address: "204 E.Piazzetta Tommaso",
                    city: "Sorrento,AZ 85022",
                    number: "(358)867-1010"
                },
                {
                    address: "Vale Puglia 54",
                    city: "Torre Del Greco AZ 85022",
                    number: "(359)867-1010"
                },
                {
                    address: "Corso Italia AA",
                    city: "Naples, AZ 85022",
                    number: "(989)867-1010"
                }
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="location">
            <img class="logo-footer" src="/img/footer-bottom-img.png" alt="">
            <div class="details-location">
                <div class="place">
                    <h4>FIND OUR RESTARAUNTS</h4>
                    <ul v-for="element in location">
                        <li>
                            {{ element.address }}
                        </li>
                        <li>
                            {{ element.city }}
                        </li>
                        <li>
                            {{ element.number }}
                        </li>
                    </ul>

                </div>
                <div>
                    <h4>WORKING HOURS</h4>
                    <ul>
                        <li><strong>MONDAY</strong></li>
                        <li class="closed">kitchen closed</li>
                        <li><strong>TUESDAY UNTIL FRIDAY</strong></li>
                        <li>9:00 - 22:00</li>
                        <li><strong>SATURDAY</strong></li>
                        <li>Saturday 11am to midnight</li>
                        <li><strong>SUNDAY</strong></li>
                        <li>9:00- 22:00</li>
                        <li><strong>FOLLOW US: </strong>
                            <a href="">
                                <i class="fa-brands fa-twitter"></i>
                            </a>
                            <a href="">
                                <i class="fa-brands fa-facebook-f"></i>
                            </a>
                            <a href="">
                                <i class="fa-brands fa-instagram"></i>
                            </a>
                            <a href="">
                                <i class="fa-brands fa-linkedin-in"></i>
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="slogan-footer">
                    <h5>THE DON PEPPE CREW FIRST AND FOREMOST VALUES AN AUTHENTIC, WELL BAKED SLICE OF PIZZA.</h5>
                </div>
            </div>
            <span class="creator">Created with &hearts; <a href="">by Qode interactive</a></span>
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


        .details-location {
            color: $white;
            padding-top: 60px;
            padding-left: 30px;
            display: flex;
            gap: 55px;

            h4,
            strong {
                color: $third-color;
                font-size: 0.7rem;
            }

            .place ul {
                margin: 20px 0;
            }


            li {
                font-size: 0.6rem;
                font-weight: 300;

                a {
                    color: $white;
                    padding: 3px;
                    display: inline-block;
                    font-size: 0.6rem;
                }
            }

            .closed {
                color: $color-price;
            }

            li strong {
                margin-top: 20px;
                display: inline-block;
            }

        }

        .slogan-footer {
            width: 29%;
            font-size: 1rem;
        }

        .logo-footer {
            width: 70px;
            position: absolute;
            bottom: 10px;
            right: 10px;

        }

        .creator {
            color: $third-color;
            font-size: 0.6rem;
            position: absolute;
            bottom: 10px;
            left: 30px;

            a {
                color: #339966;
            }
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