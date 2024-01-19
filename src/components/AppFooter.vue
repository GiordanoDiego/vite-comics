<script>
/* Come faccio ad utilizzare un componente dentro un altro?
        Si seguono 3 passaggi:
        1) Importazione del componente
        2) Dichiarazione del componente all'interno dell'oggetto
        3) Utilizzo del componente    
*/


export default {
    data(){
        return{
            shop: [
            {
                name: "DIGITAL COMICS",
                img: "/img/buy-comics-digital-comics.png"
            },
            {
                name: "DC MERCHANDISE",
                img: "/img/buy-comics-merchandise.png"
            },
            {
                name: "SUBSCRIPTION",
                img: "/img/buy-comics-subscriptions.png"
            },
            {
                name: "COMIC SHOP LOCATOR",
                img: "/img/buy-comics-shop-locator.png"
            },
            {
                name: "DC POWER VISA",
                img: "/img/buy-dc-power-visa.svg"
            },

        ],

        socials:[
                {
                    img: "/img/footer-facebook.png",
                    name: "Facebook"
                },
                {
                    img: "/img/footer-twitter.png",
                    name: "Twitter"
                },
                {
                    img: "/img/footer-youtube.png",
                    name: "Youtube"
                },
                {
                    img: "/img/footer-pinterest.png",
                    name: "Pinterest"
                },
                {
                    img: "/img/footer-periscope.png",
                    name: "Periscope"
                },            
            ],

            DC:[
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Collectibles",
                "Video",
                "Fans",
                "News"
            ]
        }
        
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
                    <div class="card" v-for="(card, i) in shop" :key="i">
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
                            <li v-for="(link, i) in DC" :key="i">
                                <a href="#">
                                    {{link}}
                                </a>
                            </li>
                        </ul>
                        
                        SHOP
                        <ul>
                            <li v-for="i in 2" :key="i">
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                       DC
                       <ul>
                            <li v-for="i in 11" :key="i">
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        SITES
                        <ul>
                            <li v-for="i in 5" :key="i">
                                <a href="#">
                                    Characters
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right_footer_2">
                    
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
                        <a href="#">FOLLOW US</a>
                    </div>
                    <div class="socials_container">
                        <div class="social_container" v-for="(social, i) in socials" :key="i">
                            <a href="#">
                                 <img :src="social.img" :alt="social.name">
                            </a>
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
