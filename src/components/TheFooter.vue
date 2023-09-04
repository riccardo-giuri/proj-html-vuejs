<script>
import NewsletterSection from './NewsletterSection.vue';

export default {
    components: {
        NewsletterSection
    },

    data() {
        return {
            icons: [
                    {code: "fa-brands fa-facebook-square", color: "#303fbf"},
                    {code: "fa-brands fa-pinterest-p", color: "#be2c4c"},
                    {code: "fa-brands fa-twitter", color: "#7ccfd3"},
                    {code: "fa-brands fa-linkedin-in", color: "#0663cf"},
                    {code: "fa-brands fa-instagram", color: "#a721b3"}
            ],

            navLinks: [
                {
                    title: "Support",
                    links: [
                        { name: "Contact Us"},
                        { name: "Online Chat"},
                        { name: "Whatsapp"},
                        { name: "Telegram"},
                        { name: "Snapchat"},
                    ]
                },
                {
                    title: "About",
                    links: [
                        { name: "About Us"},
                        { name: "Blog"},
                        { name: "Career"},
                        { name: "Job"},
                        { name: "In press"},
                    ]
                },
                {
                    title: "Faq",
                    links: [
                        { name: "Account"},
                        { name: "Order"},
                        { name: "Delivery"},
                        { name: "Payment"},
                        { name: "Return"},
                    ]
                },
            ],

            contacts: [
                    { name: "4500 Mercantile plaza,suite 300,fort worth,TX,76137,USA", icon: "fa fa-location-arrow"},
                    { name: "info@example.com", icon: "fa-solid fa-envelope"},
                    { name: "+1(817)901 3377", icon: "fa-solid fa-phone"},
            ],
        }
    }
}
</script>

<template>
    <footer>
        <NewsletterSection></NewsletterSection>

        <div class="wrapper">
            <div class="container">
                <div class="row">
                    <div class="col-3">
                        <h4>Get In Touch</h4>
                        
                        <div>Have a Question for us? <br> we'll answer your problem here</div>

                        <ul class="iconList d-flex gap-2 p-0">
                            <li v-for="icon in icons">
                                <a href="#">
                                    <span class="iconContainer" :style="{ 'backgroundColor': icon.color}"><i :class= icon.code style="color: white;"></i></span>
                                </a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-2" v-for="linksList in navLinks">
                        <h4>{{ linksList.title }}</h4>

                        <ul class="p-0 ">
                            <li v-for="link in linksList.links">
                                <a href="#">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-3">
                        <h4>Contact Me</h4>

                        <ul class="p-0">
                            <li v-for="contact in contacts" class="pb-3">
                                <a href="#">
                                    <i class="pe-2" :class= contact.icon></i>
                                </a>

                                <span> {{ contact.name }}</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="line"></div>

            <div class="copyright">
                <div class="text-center">Copyright 2022 by AttdogMilo.com</div>
            </div>
        </div>
        
    </footer>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;

    .iconContainer {
        padding: 1px 5px;
        border-radius: 5px;
    }

    li {
        list-style: none;
        padding-bottom: 6px;

        a {
            text-decoration: none;
            color: #b3b1b1;
        }
    }

    .wrapper {
        background-color: black;
        padding-top: 150px;
        padding-bottom: 10px;
    }

    h4 {
        color: map-get($map: $colorPalette, $key: "orange");
        margin-bottom: 23px;
    }

    .iconList {
        margin-top: 28px;
    }

    .col-3 {
        color: #b3b1b1;
        padding-bottom: 15px;
    }

    i {
        color: map-get($map: $colorPalette, $key: "orange");
    }

    .line {
        height: 1px;
        width: 100%;
        background-color: #857e7e61;
    }

    .copyright {
        color: white;
        margin-top: 32px;
        margin-bottom: 16px;
    }
</style>