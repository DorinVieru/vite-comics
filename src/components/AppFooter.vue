<!-- SEZIONE JS SCRIPT -->
<script>
export default {

}
</script>

<!-- SEZIONE HTML -->
<template lang="">
  <footer>

    <!-- TOP FOOTER -->
    <div class="container-fluid top-footer">
      <div class="container">
        <div class="row">
          <div class="col-2 p-4">
            <h3>DC COMICS</h3>
            <ul class="list-unstyled">
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h3 class="mt-4 mb-0">SHOP</h3>
            <ul class="list-unstyled">
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col-2 p-4">
            <h3>DC</h3>
            <ul class="list-unstyled">
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy Policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Worskshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col-2 p-4">
            <h3>SITES</h3>
            <ul class="list-unstyled">
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">Dc Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
          <div class="col-6 footer-logo"></div>
        </div>
      </div>
    </div>

    <!-- BOTTOM FOOTER -->
    <div class="container-fluid bottom-footer">
      <div class="container">
        <div class="row">
          <div class="col-6 d-flex align-items-center">
            <button type="button" class="btn btn-secondary btn-lg button-footer">SIGN-UP NOW!</button>
          </div>
          <div class="col-6 d-flex align-items-center">
            <h2>FOLLOW US</h2>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<!-- SEZIONE STYLE -->
<style lang="scss">
@use '../styles/partials/variables' as *;

  //TOP FOOTER
  .top-footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
  }

  .footer-logo{
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: right;
  }

  h3{
    color: $title_main_color !important;
    font-size: 18px !important;
    font-weight: 700 !important;
    margin-bottom: 0 !important;
  }

  ul{
    margin: 0;

    li{
      padding: 5px 0;

      a{
        color: gray;
        font-size: 13px;
        text-decoration: none;
      }
    }
  }

  //BOTTOM FOOTER
  .bottom-footer{
    background-color: $bg_footer_color;
    padding: 30px;
  }

  .button-footer{
    border: 2px solid $primary_color !important;
  }

  h2{
    color: $primary_color !important;
    font-size: 18px !important;
    font-weight: 800 !important;
    padding: 8px 10px 0;
  }

  img{
    padding: 0 10px;
  }
</style>