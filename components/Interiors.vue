<script setup lang="ts">
</script>

<template>
  <div class="interiors">
    <div  class="interiorsImages">
        <img class="interiorsImagesTitle" src="../public/interiors.svg" />
        <img class="interiorsImagesSlide" src="../public/slide.svg" />
    </div>
    <div class="interiorsPhotos">
        <img src="../public/photo-1.png" />
        <div class="swiper">
            <div class="swiperArrows">
                <div class="swiperArrowsLeft">
                    <img src="../public/swipe-arrow-left.svg" />
                </div>
                <div class="swiperArrowsRight">
                    <img src="../public/swipe-arrow.svg" />
                </div>
            </div>
            <div class="swiperCicrles">
                <div class="swiperCicrlesItem swiperCicrlesActive"></div>
                <div class="swiperCicrlesItem"></div>
                <div class="swiperCicrlesItem"></div>
                <div class="swiperCicrlesItem"></div>
                <div class="swiperCicrlesItem"></div>
                <div class="swiperCicrlesItem"></div>
            </div>
        </div>
    </div>
  </div>
</template>

<style>
    @import url("~/assets/scss/Interiors.scss");
</style>