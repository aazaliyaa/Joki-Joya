<template>
  <div class="header">
    <div><img class="headerImage" src="../public/JJ.svg" /></div>
    <div class="headerInner">
        <div>
            <div class="buttonGeo">
                <img class="buttonGeoIcon" src="../public/geo.svg" />
                <span>Москва</span>
            </div>
            <div class="buttonTel">
                <img class="buttonTelIcon" src="../public/tel.svg" />
                <span>+7 (812) 635 22 77</span>
            </div>
        </div>
        <div>
            <button class="buttonTickets">Купить билеты</button>
            <button class="buttonParty">Заказать праздник</button>
        </div>
    </div>
    <div class="menu">
        <div class="menuItem"></div>
        <div class="menuMiddleItem"></div>
        <div class="menuItem"></div>
        <div class="menuText">Меню</div>
    </div>
  </div>
  <div class="headerBorderBottom"></div>
</template>

<style>
    @import url("~/assets/scss/AppHeader.scss");
</style>