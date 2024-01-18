<script>
/* Come faccio ad utilizzare un componente dentro un altro?
        Si seguono 3 passaggi:
        1) Importazione del componente
        2) Dichiarazione del componente all'interno dell'oggetto
        3) Utilizzo del componente    
*/


export default {
    data(){
        footer1: [
            {
                name: "DIGITAL COMICS",
                img: "./img/buy-comics-digital-comics.png"
            },
            {
                name: "DC MERCHANDISE",
                img: "./img/buy-comics-merchandise.png"
            },
            {
                name: "SUBSCRIPTION",
                img: "./img/buy-comics-subscriptions.png"
            },
            {
                name: "COMIC SHOP LOCATOR",
                img: "./img/buy-comics-shop-locator.png"
            },
            {
                name: "DC POWER VISA",
                img: "./img/buy-dc-power-visa.svg"
            },

        ]
    },
   
    methods: {

    }
}


</script>

<template>
    <footer class="footer_container">
        <!-- section 1 -->
        <div class="footer_1_container">
            <div class="container_footer_1">
                <div class="cards_footer">
                    <div class="card" v-for="(card, i) in footer1">
                        <div>
                            <img :src="card.img" alt="">
                        </div>
                        <div>
                            {{card.name}}
                        </div>
                    </div>
                    
                </div>
            </div>
            
        </div>

        <!-- section 2  -->
        <div class="footer_2_container">
            <div class="container">
                <div class="left_footer_2">
                    <div>
                        DC COMICS
                        <ul>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                        
                        SHOP
                        <ul>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                       DC
                        <ul>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        SITES
                        <ul>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right_footer_2">
                    <img src="../../public/img/dc-logo-bg.png" alt="">
                </div>
            </div>
            
        </div>

        <!-- section 3 -->
        <div class="footer_3_container">
            <div class="container">
                <div class="left_footer_3">
                    <span class="link_sing_up">
                        <a href="#">
                            SING-UP NOW!    
                        </a>
                    </span>
                </div>
                <div class="right_footer_3">
                    <div class="follow_container">
                        FOLLOW US
                    </div>
                    <div class="socials_container">
                        <div class="social_container">
                        <img src="../../public/img/footer-facebook.png" alt="">
                        </div>
                        <div class="social_container">
                            <img src="../../public/img/footer-twitter.png" alt="">
                        </div>
                        <div class="social_container">
                            <img src="../../public/img/footer-youtube.png" alt="">
                        </div>
                        <div class="social_container">
                            <img src="../../public/img/footer-pinterest.png" alt="">
                        </div>
                        <div class="social_container">
                            <img src="../../public/img/footer-periscope.png" alt="">
                        </div>
                    </div>
                   
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @use'../assets/SCSS/main.scss';
    @use '../assets/SCSS/footer.scss';

</style>
