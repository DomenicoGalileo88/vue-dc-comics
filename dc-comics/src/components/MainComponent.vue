<template>
    <main class="site_main">
      <div class="main_jumbo">
      </div>
      <section class="content">
        <div class="container">
        <div class="row">
          
            <MainFigure :figure='figure' v-for="(figure, index) in main_figures" :key="index" />
            <!-- <div class="figures">
              <img :src="figure.thumb" :alt="figure.series">
              <h5 class="title_figure mt-2">{{figure.series}}</h5>
            </div> -->
          </div>
        </div>
      
      </section>
      <!-- /.content -->

      <div class="items">
        <div class="container">
          <div class="row">
          <div class="col" v-for="(item, index) in main_items" :key="index">
            <div class="img_item">
                <img :src="item.src" alt="">
                <div class="title_item">{{item.title}}</div>
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
import MainFigure from '@/components/FiguresComponent.vue';

export default {
    name:'SiteMain',
    components : {
      MainFigure
    },

    data() {
        return {
            main_items: [
            {
                src: require('@/assets/img/buy-comics-digital-comics.png'),
                title: "DIGITAL COMICS",
            },
            {
                src: require('@/assets/img/buy-comics-merchandise.png'),
                title: 'DC MERCHANDISE',
            },
            {
                src: require('@/assets/img/buy-comics-subscriptions.png'),
                title: "SUBSCRIPTION",
            },
            {
                src: require('@/assets/img/buy-comics-shop-locator.png'),
                title: "COMIC SHOP LOCATOR",
            },
            {
                src: require('@/assets/img/buy-dc-power-visa.svg'),
                title: "DC POWER VISA",
            },
        ],
            main_figures: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
        ],
        }
    }
}
</script>

<style lang="scss" scoped>
    main{
      .col_2{
        width: calc(100% / 12) * 2;
      }
      .main_jumbo{
        height: 400px;
        background-image: url('@/assets/img/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
      }
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

      .img_item {
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