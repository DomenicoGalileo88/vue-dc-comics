<template>
    <main class="site_main">
      <section class="content">
        <div class="container">
        <h2 class="title_content"> Content goes here </h2>
      </div>
      </section>
      <!-- /.content -->

      <div class="items">
        <div class="container">
          <div class="row">
          <div class="col" v-for="({src, title}, index) in main_items" :key="index">
            <div class="digital_comics">
                <img :src="require(`@/assets${src}`)" alt="">
                <div class="title_item">{{title}}</div>
            </div>
            <!-- /.digital_comics -->
          </div>

          
        </div>
        <!-- /.row -->
        </div>
        <!-- /.container -->
        
      </div>
      <!-- /.items -->

    </main>
    <!-- /.site_main -->
</template>

<script>
export default {
    name:'SiteMain',

    data() {
        return {
            main_items: [
            {
                src: "/img/buy-comics-digital-comics.png",
                title: "DIGITAL COMICS",
            },
            {
                src: '/img/buy-comics-merchandise.png',
                title: 'DC MERCHANDISE',
            },
            {
                src: "/img/buy-comics-subscriptions.png",
                title: "SUBSCRIPTION",
            },
            {
                src: "/img/buy-comics-shop-locator.png",
                title: "COMIC SHOP LOCATOR",
            },
            {
                src: "/img/buy-dc-power-visa.svg",
                title: "DC POWER VISA",
            },
        ]
        }
    }
}
</script>

<style lang="scss" scoped>
    main{
        position: relative;
        z-index: 1;
  .content{
    background-color: black;
    color: white;
    .container{
      padding: 3rem 0;
    }
  }

  .items{
    background-color: cornflowerblue;
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
        font-size: 0.9rem;
      }
    }
    }
  }

}

</style>