<template>
  <header class="site_header">
    <div class="container">
      <nav class="navbar">
        <div class="row">
          <div class="col-6 py-4">
            <div class="logo">
              <img src="@/assets/img/dc-logo.png" alt="" />
            </div>
            <!-- /.logo -->
          </div>
          <div class="col-6">
            <ul>
              <li v-for="(link, index) in nav_links" :key="index">
                <a href="#">{{ link.nome }}</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
      <!-- /.navbar -->
    </div>
    <!-- /.container -->
  </header>
  <!-- /.site_header -->
</template>

<script>
export default {
  name: "SiteHeader",
  data() {
    return {
      nav_links: [
        {
          nome: "CHARACTERS",
        },
        {
          nome: "COMMICS",
        },
        {
          nome: "MOVIES",
        },
        {
          nome: "TV",
        },
        {
          nome: "GAMES",
        },
        {
          nome: "COLLECTIBLES",
        },
        {
          nome: "VIDEOS",
        },
        {
          nome: "FANS",
        },
        {
          nome: "NEWS",
        },
        {
          nome: "SHOP",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/partials/_header.scss";
</style>