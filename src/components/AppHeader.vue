<script>
/* Come faccio ad utilizzare un componente dentro un altro?
        Si seguono 3 passaggi:
        1) Importazione del componente
        2) Dichiarazione del componente all'interno dell'oggetto
        3) Utilizzo del componente    
*/


export default {
    data(){
        return {
            links: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Collectibles",
            "Video",
            "Fans",
            "News",
            "Shop",
        ]
        }
        
    },
   
    methods: {

    }
}

</script>

<template>
     <header>
        <div class="container header_container">
            <div class="logo_header">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <div>
                <ul>
                    <li v-for="(link, i) in links" :key="i">
                        <a href="#">{{link}}</a>
                    </li>
                </ul>
            </div>
        </div>
     </header>
</template>

<style lang="scss" scoped>
    @use'../assets/SCSS/main.scss';
    @use '../assets/SCSS/header.scss';
</style>
