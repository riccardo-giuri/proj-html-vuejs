<script>
export default {

}
</script>

<template>
    <div class="background d-flex align-items-center">
        <div class="container">
            <div class="contentContainer">
                <h2>Welcome to <br> <span>DogMilo</span> Pets</h2>

                <p>Lorem Ipsum is simply dummy text of the printing <br> and typesetting industry</p>

                <button class="btn btn-primary">Get Started</button>

                <img class="btnImg" src="../assets/play.png" alt="">
            </div>
        </div>
    </div>
    
    
    
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    h2 {
        font-size: 46px;
        color: white;
        font-weight: 600;
    }

    span {
        font-size: 46px;
        color: white;
    }

    .btn-primary {
        background-color: map-get($map: $colorPalette, $key: "orange");
        border: 0;
        border-radius: 50px;
        padding: 15px 30px;
        font-size: 21px;
        font-weight: 500;
        margin-right: 12px;
    }

    p {
        padding: 14px 0 14px 0;
        font-size: 20px;
        color: white;
    }

    .background {
        background-image: url("../assets/b.png");
        background-size: cover;
        min-height: 574px;
        background-position-y: 40%;
    }

    .btnImg {
        width: 5%;
        padding: 10px 10px 10px 10px;
        background: #70d0f7;
        border-radius: 7px;
    }
</style>