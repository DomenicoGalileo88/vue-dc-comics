<template>
    <header class="site_header">
      <div class="container">
        

      <nav class="navbar">
          <div class="logo">
            <img src="@/assets/img/dc-logo.png" alt="">
        </div>
      <!-- /.logo -->
        <ul>
          <li v-for="(link, index) in nav_links" :key="index">{{link.nome}}</li>
        </ul>
      </nav>
      <!-- /.navbar -->
      </div>
      <!-- /.container -->
    </header>
    <!-- /.site_header -->
</template>

<script>
export default {
    name: 'SiteHeader', 
    data() {
        return {
            nav_links: [
                {
                    nome: 'CHARACTERS'
                },
                {
                    nome: 'COMMICS'
                },
                {
                    nome: 'MOVIES'
                },
                {
                    nome: 'TV'
                },
                {
                    nome: 'GAMES'
                },
                {
                    nome: 'COLLECTIBLES'
                },
                {
                    nome: 'VIDEOS'
                },
                {
                    nome: 'FANS'
                },
                {
                    nome: 'NEWS'
                },
                {
                    nome: 'SHOP'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

header{
        .container{
              nav{
                ul{
                  display: flex;
            
                  li{
                    font-size: 0.9rem;
                    font-weight: 600;
                    list-style: none;
                    padding: 0.5rem;
            
                    &:hover{
                        color: cornflowerblue;
                        border-bottom: 1px solid cornflowerblue;
                    }
                  }
                }
              }
        
  }
}

</style>