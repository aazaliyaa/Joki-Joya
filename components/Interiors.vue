<script setup lang="ts">
    const photoId = ref<number>(0);
    const imageUrl = ref<string>('/photo-1.png');
    const photos: string[] = [
        '/photo-1.png',
        '/photo-2.jpg',
        '/photo-3.jpeg',
        '/photo-4.jpg',
        '/photo-5.jpeg',
        '/photo-6.jpg'
    ];

    const setCicrleActive = (): void => {
        const circles =  document.querySelectorAll(".swiperCicrlesItem");
        [...circles].map(elem => {
            elem.classList.remove("swiperCicrlesActive");
        });
        [...circles][photoId.value].classList.add("swiperCicrlesActive")
    }

    const handleSwipeRight = (): void => {
       if (photoId.value < photos.length-1) {
           photoId.value++;
           imageUrl.value = photos[photoId.value];
           setCicrleActive();
       }
    };
    const handleSwipeLeft = (): void => {
        if (photoId.value > 0) {
            photoId.value--;
            imageUrl.value = photos[photoId.value];
            setCicrleActive();
        }
    };
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
        <img class="interiorsPhotosDesktop" :src="imageUrl" />
        <img class="interiorsPhotosMobile" src="../public/mobile-photo-1.png" />
        <div class="swiper">
            <div class="swiperArrows">
                <div class="swiperArrowsLeft" @click="handleSwipeLeft()">
                    <img src="../public/swipe-arrow-left.svg" />
                </div>
                <div class="swiperArrowsRight" @click="handleSwipeRight()">
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