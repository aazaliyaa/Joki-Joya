<script setup lang="ts">
</script>

<template>
  <div class="page">
    <AppHeader />
    <Sidebar />
    <MainImage />
    <AppTitle />
    <div class="pageBody">
        <img class="verticalImage" src="../public/vertical-image.svg" />
        <div>
            <Description />
            <Facts />
        </div>
    </div>
    <Interiors />
  </div>
</template>

<style>
    @import url("~/assets/scss/MainPage.scss");
</style>