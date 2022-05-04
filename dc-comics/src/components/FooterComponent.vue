<template>
  <footer class="site_footer">
    <section class="utyls">
      <div class="container">
        <div class="row">
          <div class="col-2 py-4">
            <ul>
              <h5 class="title_utyls">DC COMICS</h5>
              <li v-for="(utyl, index) in comics_utyls" :key="index">
                {{ utyl.link }}
              </li>
            </ul>

            <ul>
              <h5 class="title_utyls">SHOP</h5>
              <li v-for="(utyl, index) in shop_utyls" :key="index">
                {{ utyl.link }}
              </li>
            </ul>
          </div>
          <!-- /.col-1 -->
          <div class="col-2 py-4">
            <ul>
              <h5 class="title_utyls">DC</h5>
              <li v-for="(utyl, index) in dc_utyls" :key="index">
                {{ utyl.link }}
              </li>
            </ul>
          </div>
          <!-- /.col-1 -->
          <div class="col-2 py-4">
            <ul>
              <h5 class="title_utyls">SITES</h5>
              <li v-for="(utyl, index) in sites_utyls" :key="index">
                {{ utyl.link }}
              </li>
            </ul>
          </div>
          <!-- /.col-1 -->

          <div class="col-6 logo_big">
            <img src="@/assets/img/dc-logo-bg.png" alt="" />
          </div>
          <!-- /.col-6 -->
        </div>
      </div>
    </section>
    <!-- /.utyls -->

    <section class="follows">
      <div class="container">
        <div class="sign">
          <button class="btn-outline-pimary">SIGN-UP NOW!</button>
        </div>
        <div class="follow_us">
          <h5 class="title_follow_us">FOLLOWS US</h5>
          <div
            v-for="(icon, index) in icons_footer"
            :key="index"
            class="icon_follows"
          >
            <img :src="icon.icon" alt="" />
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
  name: "SiteFooter",
  data() {
    return {
      comics_utyls: [
        {
          link: "Characters",
        },
        {
          link: "Comics",
        },
        {
          link: "Movies",
        },
        {
          link: "TV",
        },
        {
          link: "Games",
        },
        {
          link: "Videos",
        },
        {
          link: "News",
        },
      ],
      shop_utyls: [
        {
          link: "Shop DC",
        },
        {
          link: "Shop DC Collectibles",
        },
      ],
      dc_utyls: [
        {
          link: "Ters Of Use",
        },
        {
          link: "Privacy policy",
        },
        {
          link: "Ad Choices",
        },
        {
          link: "Adversting",
        },
        {
          link: "Jobs",
        },
        {
          link: "Subscription",
        },
        {
          link: "Talent Workshop",
        },
        {
          link: "CPSC Certificates",
        },
        {
          link: "Ratings",
        },
        {
          link: "Shop Help",
        },
        {
          link: "Contact Us",
        },
      ],
      sites_utyls: [
        {
          link: "DC",
        },
        {
          link: "MAD Magazine",
        },
        {
          link: "DC Kids",
        },
        {
          link: "DC Universe",
        },
        {
          link: "DC Power Vista",
        },
      ],
      icons_footer: [
        {
          icon: require("@/assets/img/footer-facebook.png"),
        },
        {
          icon: require("@/assets/img/footer-twitter.png"),
        },
        {
          icon: require("@/assets/img/footer-youtube.png"),
        },
        {
          icon: require("@/assets/img/footer-pinterest.png"),
        },
        {
          icon: require("@/assets/img/footer-periscope.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/partials/_footer.scss";
</style>
