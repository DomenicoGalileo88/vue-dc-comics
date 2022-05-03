<template>
    <header class="site_header">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="">
      </div>
      <!-- /.logo -->

      <nav class="navbar">
        <ul>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ul>
      </nav>
      <!-- /.navbar -->
    </header>
    <!-- /.site_header -->
</template>

<script>
export default {
    name: 'SiteHeader'
}
</script>

<style lang="scss" scoped>

header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  nav{
    ul{
      display: flex;

      li{
        list-style: none;
        padding: 1rem;
      }
    }
  }
}

</style>