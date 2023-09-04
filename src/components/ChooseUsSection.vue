<script>
export default {

}
</script>

<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-6">
                <img class="sectionImg" src="../assets/why.png" alt="">
            </div>

            <div class="col-6 left-col">

                <div class="IconTitle d-flex align-items-center">
                    <img src="../assets/dog-icon.png" alt="">
                    <h6>Choose us</h6>
                </div>

                <h2>Why Choose Us?</h2>

                <div class="chooseOption d-flex">
                    <img class="chooseImg" src="../assets/w-3.png" alt="">

                    <div class="textOption">
                        <h3>Safety First</h3>

                        <p>It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                    </div>
                </div>

                <div class="chooseOption d-flex middleOption">
                    <img class="chooseImg" src="../assets/w-2.png" alt="">

                    <div class="textOption">
                        <h3>Play Yards</h3>

                        <p>It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                    </div>
                </div>

                <div class="chooseOption d-flex lastOption">
                    <img class="chooseImg" src="../assets/w-1.png" alt="">

                    <div class="textOption">
                        <h3>Monitor Your Pets</h3>

                        <p>It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .sectionImg {
        width: 100%;
    }

    .col-6 {
        padding: 0;
    }

    .left-col {
        padding-left: 55px;
        padding-right: 90px;
        padding-top: 70px;
    }

    .chooseOption {
        img {
            width: 158px;
            margin-right: 20px;
        }
    }

    .textOption {
        h3 {
            font-size: 24px;
            font-style: 500;
        }

        p {
            font-size: 18px;
            padding-top: 10px;
        }
    }

    .middleOption {
        margin-left: 160px;
    }

    .lastOption {
        margin-left: 330px;
    }

    .IconTitle {
        margin-bottom: 20px;

        img {
            width: 76px;
            padding-right: 14px;
        }

        h6 {
            font-size: 16pz;
            color: map-get($map: $colorPalette, $key: "mossBrown");
        }
    }

    h2 {
        font-size: 40px;
        margin-bottom: 36px;
    }
</style>