<script>
export default {

}
</script>

<template>
    <section class="WelcomePets">
        <div class="dogImgContainer">
            <img class="dogImg" src="../assets/dog-logo.png" alt="">
        </div>

        <div class="container">
            <div class="row">
                <div class="col-6">
                    <img class="mainImg" src="../assets/about.png" alt="">
                </div>

                <div class="col-6 textContainer">
                    <div class="titleContainer">
                        <img src="../assets/dog-icon.png" alt="">
                        <span class="title">About Us</span>
                    </div>

                    <h2>Welcome DogMilio Pets</h2>

                    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled</p>

                    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .title {
        color: map-get($map: $colorPalette, $key: "mossBrown");
        font-weight: 500;
        padding-left: 14px;
    }

    .titleContainer {
        margin-bottom: 28px;
    }

    h2 {
        margin-bottom: 28px;
        font-size: 40px;
    }

    p {
        margin-bottom: 16px;
        font-size: 18px;
    }

    .mainImg {
        width: 90%;
    }

    .WelcomePets {
        padding: 90px 0px;
    }

    .textContainer {
        padding: 90px 0 0 20px;
    }

    .dogImgContainer {
        left: 87%;
        position: absolute;
    }

    .dogImg {
        width: 100%;
    }
</style>