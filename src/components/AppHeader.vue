<script>
/* Come faccio ad utilizzare un componente dentro un altro?
        Si seguono 3 passaggi:
        1) Importazione del componente
        2) Dichiarazione del componente all'interno dell'oggetto
        3) Utilizzo del componente    
*/


export default {
    data(){
        link: [
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
    },
   
    methods: {

    }
}

</script>

<template>
     <header>
        <div class="container header_container">
            <div class="logo_header">
                <img src="../../public/img/dc-logo.png" alt="">
            </div>
            <div>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Collectibles</a>
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
