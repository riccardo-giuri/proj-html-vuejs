<script>
export default {
    data() {
        return {

            primaryNav: {
                dropDowns: [
                {
                    name: "Home", 
                    options: [ 
                        { title: "Home One"},
                        { title: "Home Two"}
                    ]  
                }
                ],

                Links: [
                { name: "About"},
                { name: "Services"},
                { name: "Training"},
                { name: "Blogs"}
                ],

                buttons: [
                    { name: "Get in Touch!"}
                ]
            }        
        }
    }
}
</script>

<template>
    <header>
        <div class="primaryNav">
            <nav class="navbar justify-content-between">
                <a class="navbar-brand" href="index.html">
                    <img src="../assets/logo.png" alt="">
                </a>  

                <div class="d-flex gap-5">
                    <ul class="navbar-nav flex-row">
                        <li class="nav-item dropdown" v-for="dropdown in primaryNav.dropDowns">
                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="true">
                                {{ dropdown.name }}
                            </a>
                            <ul class="dropdown-menu" >
                                <li v-for="option in dropdown.options">
                                    <a class="dropdown-item" href="#">{{ option.title }}</a>
                                </li>
                            </ul>
                        </li>

                        <li class="nav-item">
                            <a class="nav-link" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Features</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Pricing</a>
                        </li>
                    </ul>

                    <button class="btn btn-primary " v-for="button in primaryNav.buttons"> {{ button.name }}</button>
                </div>


            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .dropdown-menu {
        position: absolute;
    }

    .nav-item {
        padding: 0 0px 0 40px;
        font-size: 21px;
        font-weight: 500;
    }

    .btn-primary {
        background-color: map-get($map: $colorPalette, $key: "orange");
        border: 0;
        border-radius: 50px;
        padding: 12px 25px;
        font-size: 21px;
        font-weight: 500;
    }
</style>