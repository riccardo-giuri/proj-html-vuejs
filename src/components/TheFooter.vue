<script>
export default {

}
</script>

<template>
    <footer>
        <div class="container">
            <div class="contentNewsletter">
                <div class="row">
                    <div class="col-6 position-relative">
                        <img src="../assets/news.png" alt="">
                    </div>

                    <div class="col-6">
                        <h4>Subscribe to Our Newsletter</h4>
                        <form action="" class="form d-flex" >
                            <input type="email" name="email" placeholder="Your Email Here">
                            <button class="form-button">
                                <i class="fa fa-at"></i>
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>

        
    </footer>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .content {
        margin-left: 114px;
        margin-right: 114px;
    }

    .col-6 {
        img {
            position: absolute;
            left: 65px;
            bottom: 0px;
            width: 340px;
            height: 295px;
            width: auto;
        }
    }

    form {
        border: 3px solid white;
        margin-bottom: 45px;

        input {
            width: 100%;
            height: 58px;
            border: none;
            padding: 10px 20px;
        }
    }

    .form-button {
        background: map-get($map: $colorPalette, $key: "orange");
        border: none;
        color: #fff;
        font-size: 27px;
        padding: 10px;
        width: 52px;
        height: 52px;
    }

    .row {
        background-color: map-get($map: $colorPalette, $key: "orange");
        border-radius: 10px;
    }

    h4 {
        padding-top: 50px;
        padding-bottom: 18px;
    }
</style>