<template>
    <footer class="site_footer">

      <section class="utyls">
        <div class="container">
          <div class="row">
            <div class="col-2 py-4">
              <ul>
                <h5 class="title_utyls">DC COMICS</h5>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
              </ul>

              <ul>
                <h5 class="title_utyls">SHOP</h5>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </div>
            <!-- /.col-1 -->
            <div class="col-2 py-4">
              <ul>
                <h5 class="title_utyls">DC</h5>
                <li>Ters Of Use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Adversting</li>
                <li>Jobs</li>
                <li>Subscription</li>
                <li>Talent Workshop</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </div>
            <!-- /.col-1 -->
            <div class="col-2 py-4">
              <ul>
                <h5 class="title_utyls">SITES</h5>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Vista</li>
              </ul>
            </div>
            <!-- /.col-1 -->

            <div class="col logo_big">
              <img src="@/assets/img/dc-logo-bg.png" alt="">
            </div>
            <!-- /.col-6 -->
          </div>
        </div>
      </section>
      <!-- /.utyls -->

      <section class="follows">
        <div class="container">
          <div class="sign">
            <button>SIGN-UP NOW!</button>
          </div>
          <div class="follow_us">
            <h3 class="title_follow_us">FOLLOWS US</h3>
            <div class="icon_follows">
              <img src="@/assets/img/footer-facebook.png" alt="">
              <img src="@/assets/img/footer-twitter.png" alt="">
              <img src="@/assets/img/footer-youtube.png" alt="">
              <img src="@/assets/img/footer-pinterest.png" alt="">
              <img src="@/assets/img/footer-periscope.png" alt="">

            </div>
          </div>
        </div>
      </section>
      <!-- /.follow -->

    </footer>
    <!-- /.site_footer -->
</template>

<script>
export default {
    name: 'SiteFooter',
}
</script>

<style lang="scss" scoped>
footer{
  .utyls{
    ul{
      padding-left: 0;
    }
    background-image: url('@/assets/img/footer-bg.jpg');
    li{
      color: grey;
      list-style: none;
    }
    .title_utyls{
      color: white;
      margin-bottom: 1rem;
    }

    .logo_big{
      display: flex;
      align-items: center;
        img{
          padding-left: 8rem;
          height: 110%;
        }
      }
  }

  .follows{
    padding: 3rem 0;
      background-color: rgb(77, 77, 77);
    .container{
      display: flex;
      justify-content: space-between;
      
      button{
        background-color: transparent;
        border: 1px solid blue;
        padding: 0.5rem;
        color: white;
        font-size: bold;
      }
  
      .title_follow_us{
        color: blue;
      }

      .follow_us{
        display: flex;
        .icon_follows{
          img{
            margin-left: 0.5rem;
          }
        }
      }
    }
  }
}

</style>