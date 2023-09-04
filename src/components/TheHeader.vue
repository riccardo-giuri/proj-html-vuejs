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
            },   
            
            secondaryNav: {
                contacts: [
                    { name: "info@example.com", icon: "fa-solid fa-envelope"},
                    { name: "+1(817)901 3377", icon: "fa-solid fa-phone"},
                ],

                icons: [
                    {code: "fa-brands fa-facebook-square", color: "#303fbf"},
                    {code: "fa-brands fa-pinterest-p", color: "#be2c4c"},
                    {code: "fa-brands fa-twitter", color: "#7ccfd3"},
                    {code: "fa-brands fa-linkedin-in", color: "#0663cf"},
                    {code: "fa-brands fa-instagram", color: "#a721b3"}
                ]
            }
        }
    }
}
</script>

<template>
    <header>
        <div class="secondaryNav d-flex justify-content-between">
            <div class="container d-flex justify-content-between align-items-center">
                <ul class="d-flex gap-4 m-0 text-light">
                    <li v-for="contact in secondaryNav.contacts">
                        <a href="#">
                            <i class="contactIcon" :class= contact.icon></i>
                        </a>

                        <span> {{ contact.name }}</span>
                    </li>
                </ul>

                <ul class="iconList d-flex gap-2 m-0">
                    <li v-for="icon in secondaryNav.icons">
                        <a href="#">
                            <span class="iconContainer" :style="{ 'backgroundColor': icon.color}"><i :class= icon.code style="color: white;"></i></span>
                        </a>
                    </li>
                </ul>
            </div>
            
        </div>

        <div class="primaryNav">
            <div class="container">
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

                        <li class="nav-item" v-for="link in primaryNav.Links">
                            <a class="nav-link" href="#">{{ link.name }}</a>
                        </li>
                    </ul>

                    <button class="btn btn-primary " v-for="button in primaryNav.buttons"> {{ button.name }}</button>
                </div>
            </nav>
            </div>
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

        a:hover {
            color: map-get($map: $colorPalette, $key: "orange");
        }
    }

    .btn-primary {
        background-color: map-get($map: $colorPalette, $key: "orange");
        border: 0;
        border-radius: 50px;
        padding: 12px 25px;
        font-size: 21px;
        font-weight: 500;
    }

    .contactIcon {
        color: map-get($map: $colorPalette, $key: "orange");
        padding-right: 8px;
    }

    li {
        list-style: none;
    }

    .socialIcon {
        padding-right: 8px;
    }

    .secondaryNav {
        background-color: map-get($map: $colorPalette, $key: "mossBrown");
        min-height: 55px;
    }

    .iconList {
        padding-right: 15px;
    }

    .iconContainer {
        padding: 1px 5px;
        border-radius: 5px;
    }

    .nav-link {
        color: #0000007a;
        font-size: 21px;
        font-weight: 500;
    }

    button:hover {
        background: #173b67;
    }
</style>