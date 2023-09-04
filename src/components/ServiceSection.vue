<script>
import Card from "./Card.vue";
import {store} from "../store";

export default {
    components:{
        Card
    },

    data() {
        return {
            store
        }
    }
}
</script>

<template>
    <section class="service">
        <div class="dogImgContainer">
            <img class="dogImg" src="../assets/dog-logo.png" alt="">
        </div>

        <div class="dogImgContainerleft">
            <img class="dogImgleft" src="../assets/dog-left.png" alt="">
        </div>

        <h6>Service</h6>

        <h2>DogMilo Pet Care Service <br> For Your Best Friends.</h2> 

        <div class="container">
            <div class="row">
                <div class="col-20" v-for="card in store.cardsData">
                    <Card :singleCardData='card'></Card>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .col-20 {
        width: 18%;
        margin: 0px 10px;
    }

    h2 {
        text-align: center;
        margin-bottom: 24px;
    }

    h6 {
        text-align: center;
        margin-bottom: 38px;
    }

    .dogImgContainer {
        left: 87%;
        position: absolute;
    }

    .dogImgContainerleft {
        left: 0%;
        position: absolute;
    }

    .dogImg {
        width: 100%;
    }

    .dogImgleft {
        width: 60%;
    }

    .service {
        background-color: map-get($map: $colorPalette, $key: "dirtyWhite");
        padding: 60px 0px;
    }
</style>