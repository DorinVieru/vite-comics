<!-- SEZIONE JS SCRIPT -->
<script>
import AppCard from '../components/AppCard.vue'
import AppJumbo from '../components/AppJumbo.vue'

export default {
    name: "AppMain",
    components:{
        AppCard,
        AppJumbo,
    },
    data() {
        return {
            comics: [
                    {
                        "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                        "price": "$19.99",
                        "series": "Action Comics",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                        "price": "$3.99",
                        "series": "American Vampire 1976",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                        "price": "$16.99",
                        "series": "Aquaman",
                        "type": "graphic novel",
                    },
                    {
                        "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                        "price": "$2.99",
                        "series": "Batgirl",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                        "price": "$3.99",
                        "series": "Batman",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                        "price": "$2.99",
                        "series": "Batman Beyond",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                        "price": "$3.99",
                        "series": "Batman/Superman",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                        "price": "$4.99",
                        "series": "Batman/Superman Annual",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                        "price": "$5.99",
                        "series": "Batman: The Joker War Zone",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                        "price": "$6.99",
                        "series": "Batman: Three Jokers",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                        "price": "$4.99",
                        "series": "Batman: White Knight Presents: Harley Quinn",
                        "type": "comic book",
                    },
                    {
                        "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                        "price": "$16.99",
                        "series": "Catwoman",
                        "type": "graphic novel",
                    },
            ]
        }
    },
}
</script>

<!-- SEZIONE HTML -->
<template lang="">

<!-- SECTION JUMBOTRON -->
<section>
    <AppJumbo></AppJumbo>
</section>

<!-- MAIN -->
  <main class="d-flex align-items-center">
    <div class="container">
        <div class="row">
            <!-- COMIC CARD -->
           <!-- COMICS CARD COMPONENT -->
                    <AppCard class="my-4" v-for="(comic, index) in comics" :key="index" :comic="comic"></AppCard>

                    <div class="text-center mt-3 mb-5">
                        <button type="button" class="btn btn-primary">LOAD MORE</button>
                    </div>
        </div>
    </div>
</main>

<!-- SECTION BG BLUE -->
<div class="container-fluid py-5 bg-blu-icon">
    <div class="container">
        <div class="row justify-content-around">
            <div class="col-2 d-flex align-items-center px-0">
                <div>
                    <img class="img-main" src="../assets/img/buy-comics-digital-comics.png" alt="">
                </div> 
                <div>
                    <h6>DIGITAL COMICS</h6>
                </div>
            </div>
            <div class="col-2 d-flex align-items-center px-0">
                <div>
                    <img class="img-main" src="../assets/img/buy-comics-merchandise.png" alt="">
                </div> 
                <div>
                    <h6>DC MERCHANDISE</h6>
                </div>
            </div>
            <div class="col-2 d-flex align-items-center px-0">
                <div>
                    <img class="img-main" src="../assets/img/buy-comics-subscriptions.png" alt="">
                </div> 
                <div>
                    <h6>SUBSCRIPTION</h6>
                </div>
            </div>
            <div class="col-2 d-flex align-items-center px-0">
                <div>
                    <img class="img-main" src="../assets/img/buy-comics-shop-locator.png" alt="">
                </div> 
                <div>
                    <h6>COMIC SHOP LOCATOR</h6>
                </div>
            </div>
            <div class="col-2 d-flex align-items-center px-0">
                <div>
                    <img class="img-main" src="../assets/img/buy-dc-power-visa.svg" alt="">
                </div> 
                <div>
                    <h6>DC POWER VISA</h6>
                </div>
            </div>
        </div>
    </div>
</div>  
</template>

<!-- SEZIONE STYLE -->
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    main{
        background-color: $bg-main-color;
        padding-top: 30px;
    }

    h1{
        color: $title_main_color;
    }

// SECTION BG-BLUE
    .bg-blu-icon{
        background-color: $primary_color;
    }

    h6{
        color: $title_main_color !important;
        font-size: 13px !important;
        margin: 0 0 0 5px;
    }

    .img-main{
        width: 50px;
        padding: 0;
    }
</style>