<script setup lang="ts">
</script>

<template>
  <div class="page">
    <div  class="pageBackground">
        <AppHeader />
        <MainImage />
        <Sidebar />
        <AppTitle />
        <div class="pageBody">
            <img class="verticalImage" src="../public/vertical-image.svg" />
            <div>
                <Description />
                <Facts />
            </div>
        </div>
    </div>
    <Interiors />
    <AppFooter />
  </div>
</template>

<style>
    @import url("~/assets/scss/MainPage.scss");
</style>