<script>
export default {
    props: {
        singleCardData: {
            type: Object,
            required: true
        }
    }
}
</script>

<template>
    <div class="petCard d-flex flex-column align-items-center">
        <img class="petImg" :src='`/src/assets/${singleCardData.img}`' alt="">

        <h4>{{ singleCardData.title }}</h4>

        <p>{{ singleCardData.paragraph }}</p>

        <div class="arrowLink">
            <a class="d-flex justify-content-center align-items-center" href="#"><img class="arrow-img" src="../assets/right.png" alt=""></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .arrowLink {
        height: 50px;
        width: 50px;
        border-radius: 50%;
        background-color: map-get($map: $colorPalette, $key: "yellow");;
    }

    .arrow-img {
        width: 26px;
        padding: 5px;
        vertical-align: middle;
    }

    a {
        height: 100%;
        width: 100%;
    }

    .petCard {
        color: white;
        background-color: map-get($map: $colorPalette, $key: "orange");
        border-radius: 99px 99px 99px 99px;
        padding: 20px 15px 20px 15px;
    }

    .petImg {
        width: 70px;
        margin-bottom: 10px;
    }

    p {
        text-align: center;
        font-size: 16px;
    }

    h4 {
        text-align: center;
        font-size: 18px;
    }
</style>