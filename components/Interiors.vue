<script setup lang="ts">
</script>

<template>
  <div class="interiors">
    <div  class="interiorsImages">
        <!-- svg for desktop has extra spaces -->
        <div class="interiorsImagesTitleBox">
            <img class="interiorsImagesTitle" src="../public/interiors-title.png" />
        </div>
        <div>
            <img class="interiorsImagesSlide" src="../public/slide.svg" />
        </div>
    </div>
    <div class="interiorsTitleMobile">
        <img src="../public/mobile-interiors.png" />
    </div>
    <div class="interiorsPhotos">
        <img class="interiorsPhotosDesktop" src="../public/photo-1.png" />
        <img class="interiorsPhotosMobile" src="../public/mobile-photo-1.png" />
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