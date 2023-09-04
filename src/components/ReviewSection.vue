<script>
export default {

}
</script>

<template>
    <section class="review">
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="iconTitle d-flex align-items-center">
                        <img src="../assets/dog-icon.png" alt="">
                        <h6>Review & Rating</h6>
                    </div>

                    <h2>Over 8000 Customers With 5-Star Review</h2>

                    <p>It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>

                    <ul class="rating">
                        <li><i class="fa fa-star"></i></li>
                        <li><i class="fa fa-star"></i></li>
                        <li><i class="fa fa-star"></i></li>
                        <li><i class="fa fa-star"></i></li>
                        <li><i class="fa fa-star"></i></li>
                    </ul>
                </div>

                <div class="col-8 d-flex justify-content-between">
                    <div class="reviewCard">
                        <ul class="rating">
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                        </ul>

                        <h4>Great Place</h4>

                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when</p>

                        <div class="infoReview d-flex align-items-center gap-3">
                            <img src="../assets/t1.png" alt="">

                            <div class="reviewUser">
                                <h4>Tobias May</h4>
                                <p>UI/UX Designer</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="reviewCard">
                        <ul class="rating">
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                            <li><i class="fa fa-star"></i></li>
                        </ul>

                        <h4>Great Place</h4>

                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when</p>

                        <div class="infoReview d-flex align-items-center gap-3">
                            <img src="../assets/t1.png" alt="">

                            <div class="reviewUser">
                                <h4>Tobias May</h4>
                                <p>UI/UX Designer</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="arrowbtns mt-3 d-flex justify-content-end gap-3">
                    <button class="btn">
                        <img src="../assets/left-arrow.png" alt="">
                    </button>
                    <button class="btn">
                        <img src="../assets/next.png" alt="">
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .rating {
        display: flex;
        color: gold;
        list-style: none;
        padding: 0;
    }

    .iconTitle {
        color: map-get($map: $colorPalette, $key: "mossBrown");

        img {
            width: 22px;
            height: 22px;
            margin-right: 14px;
        }

        h6 {
            margin: 0;
        }
    }

    h2 {
        margin-top: 20px;
        margin-bottom: 28px;
    }

    .col-4 {
        p {
            margin-bottom: 31px;
        }
    }
    .reviewCard {
        padding-left: 20px;
        padding-top: 20px;
        padding-right: 20px;
        width: 360px;
        min-height: 300px;
        background-color: map-get($map: $colorPalette, $key: "dirtyWhite");

        h4 {
            font-size: 20px;
            margin-bottom: 18px;
        }
    }

    .col-8 {
        p {
            margin-bottom: 26px;
        }
    }

    .infoReview {
        img {
            width: 16%;
            height: 16%;
            border-radius: 50%;
        }
    }

    .reviewUser {
        h4 {
            margin: 0;
        }

        p {
            font-size: 17px;
            margin: 0;
        }
    }

    .review {
        padding: 90px 0;
    }

    button {
        padding: 0;
        border: 0;
    }

    .btn {
        img {
            width: 39px;
            padding: 6px;
            background-color: map-get($map: $colorPalette, $key: "orange");

            &:hover {
                background-color: map-get($map: $colorPalette, $key: "mossBrown");
            }
        }
    }
</style>