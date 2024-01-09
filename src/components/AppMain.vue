<!-- SEZIONE JS SCRIPT -->
<script>
export default {
    name: "AppMain",
    data() {
        return {
            
        }
    },
}
</script>

<!-- SEZIONE HTML -->
<template lang="">

<!-- MAIN -->
  <main class="d-flex align-items-center">
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1 > --> Content goes here <-- </h1>
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