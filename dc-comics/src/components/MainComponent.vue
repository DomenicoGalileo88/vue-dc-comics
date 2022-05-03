<template>
    <main class="site_main">
      <section class="content">
        <div class="container">
        <h2 class="title_content"> Content goes here </h2>
      </div>
      </section>
      <!-- /.content -->

      <section class="items">
        <div class="container">
          <div class="row">
          <div class="col">
            <div class="digital_comics">
                <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
                <h6 class="title_item">DIGITAL COMICS</h6>
            </div>
            <!-- /.digital_comics -->
          </div>

          <div class="col">
            <div class="merchandise">
              <img src="@/assets/img/buy-comics-merchandise.png" alt="">
                <h6 class="title_item">DIGITAL COMICS</h6>
            </div>
            <!-- /.merchandise -->
          </div>

          <div class="col">
            <div class="subscription">
              <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
                <h6 class="title_item">DIGITAL COMICS</h6>
            </div>
            <!-- /.subscription -->
          </div>

          <div class="col">
            <div class="shop">
              <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
                <h6 class="title_item">DIGITAL COMICS</h6>
            </div>
            <!-- /.shop -->
          </div>

          <div class="col">
            <div class="power">
              <img src="@/assets/img/buy-dc-power-visa.svg" alt="">
                <h6 class="title_item">DIGITAL COMICS</h6>
            </div>
            <!-- /.power -->
          </div>
        </div>
        </div>
        
      </section>
      <!-- /.items -->

    </main>
    <!-- /.site_main -->
</template>

<script>
export default {
    name:'SiteMain'
}
</script>

<style lang="scss" scoped>
    main{
  .content{
    background-color: black;
    color: white;
    .container{
      padding: 3rem 0;
    }
  }

  .items{
    background-color: blue;
    color: white;
    img{
      height: 60px;
    }
    
    .container{
      padding: 3rem 3rem;

      .digital_comics, .merchandise, .subscription, .shop, .power {
      display: flex;
      align-items: center;
      .title_item{
        margin-left: 0.7rem;
      }
    }
    }
  }

}

</style>