<template>
    <div class="cards_container">

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/895786_7b4b_2-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> The Complete iOs 10 & Swift 3 Developer Course </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star-half-stroke"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$</span>199.99
                        </div>
                        <div class="new_price">$100</div>
                    </span>
                </div>
            </div>
        </div>

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/246154_d8b0_3-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> Web Design for Beginners: Real World Coding in HTML & CSS </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star-half-stroke"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$</span>129.99
                        </div>
                        <div class="new_price">$65</div>
                    </span>
                </div>
            </div>
        </div>

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/752950_b773-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> GitHub Ultimate: Master Git and GitHub - Beginner to Expert </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-regular fa-star"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$</span>99.99
                        </div>
                        <div class="new_price">$50</div>
                    </span>
                </div>
            </div>
        </div>

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/1253188_58f7_2-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> The Complete iOS 11 & Swift Developer Course - Build 20 Apps </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-regular fa-star"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$</span>199.99
                        </div>
                        <div class="new_price">$100</div>
                    </span>
                </div>
            </div>
        </div>

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/919872_ed54_6-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> Android Java Masterclass - Become an App Developer </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star-half-stroke"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$99.99</span>
                        </div>
                        <div class="new_price">$50</div>
                    </span>
                </div>
            </div>
        </div>

        <!-- CARD -->
        <div class="card">
            <div class="card_img_area">
                <!--immagine-->
                <img src="@/assets/img/951684_9c1a_2-544x322.jpg" alt="">
            </div>
            <div class="card_info_area">
                <!-- genere -->
                <p class="genre"> Development > </p>
                <!-- titolo -->
                <p> Xamarin Forms: Build Native Cross-platform Apps with C# </p>
                <div class="separator"></div>
                <div class="bottom_area">
                    <span class="stars">
                        <!--stars-->
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-regular fa-star"></i>
                    </span>
                    <span class="prices">
                        <div class="old_price">
                            <span>$</span>189.99
                        </div>
                        <div class="new_price">$95</div>
                    </span>
                </div>
            </div>
        </div>

        


    </div>



</template>

<script>


export default {
    name: "PopularCardsDevComponent",
}
</script>

<style lang="scss" scoped>
.cards_container {
    display: flex;
    flex-wrap: wrap;
    column-gap: 15px;
    row-gap: 15px;
}

.card {
    width: calc(100% / 6 - 15px);
    border: 1px solid grey;

    .separator {
        margin-bottom: 5px;
    }

    .card_info_area {
        padding-left: 10px;
        padding-right: 10px;
        padding-bottom: 10px;
        font-size: 0.85rem;

        .genre {
            font-size: 0.7rem;
            color: grey;
        }
    }

    .bottom_area {
        display: flex;
        justify-content: space-between;
    }

    .stars {
        color: #efb467;
        margin: 5px 0px;
    }

    .prices {
        text-align: right;

        .old_price {
            font-size: 0.7rem;
            color: grey;
            text-decoration: line-through;
        }

        .new_price {
            font-weight: 600;
        }
    }
}
</style>