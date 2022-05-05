<template>
<div class="col_2">
  <div class="figures">
      <img :src="figure.thumb" :alt="figure.series">
      <h5 class="title_figure mt-2">{{figure.series}}</h5>
  </div>
</div>
</template>

<script>
export default {
    name: 'MainFigure',
    props: {
      figure: Object,
    }
}
</script>

<style lang="scss" scoped>
  .figures{
    text-align: center;
      img{
          aspect-ratio: 1/1;
          height: 200px;
          object-fit: cover;
          object-position: top;
        }
      }
</style>