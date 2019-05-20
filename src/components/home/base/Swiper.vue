<template>
    <div class="swiper">
      <swiper :options="swiperOption">
        <swiper-slide v-for="swiperItem in swiperList">
          <img :src="swiperItem" alt="">
        </swiper-slide>
        <div class="swiper-pagination"  slot="pagination"></div>
      </swiper>
    </div>
</template>

<script>
  export default {
    name: 'HomeSwiper',
    data() {
      return {
        swiperList:[
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20195/60904fc24f223e0db5aee3c6148e641f.jpg_750x200_b1b90a19.jpg',
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/d7bbc21db442366a882e04ddc984669a.jpg_750x200_85e640d9.jpg',
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/87a224d0349d94a11e97f31aa1aba4f5.jpg_750x200_1f78af87.jpg',
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/437a486a1627adae39ab30e4d98fbcee.jpg_750x200_d8477149.jpg',
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20195/e4a4bf3cf8a2db15ec11a82f78d49901.jpg_750x200_f3de96e6.jpg',
          'http://img1.qunarzz.com/piao/fusion/1807/5e/cfee2e9e2f357202.jpg_750x200_b0308a43.jpg',
          'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/7bf2c282e2e57d165164ffd4b355acae.jpg_750x200_487998a6.jpg'
        ],
        swiperOption: {
          pagination: {
            el: '.swiper-pagination'
          }
        }
      }
    }
  }
</script>

<style lang="stylus" scoped>
  .swiper>>>.swiper-pagination-bullet-active
    background-color rgba(255,255,255,1)
  .swiper
    height 2.19rem
    img
      height 100%
      width 100%
</style>
