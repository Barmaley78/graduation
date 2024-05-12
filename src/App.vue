<template>
  <div id="app">
    <header class="header center">
      <img src="./assets/images/Logo.svg" alt="company logo" class="header__logo">
      <div class="header__categories">
        <span class="header__categories-item">Наши услуги</span>
        <span class="header__categories-item">О компании</span>
        <span class="header__categories-item">Отзывы</span>
        <span class="header__categories-item">Выполненные заказы</span>
        <span class="header__categories-item">Контакты</span>
      </div>
      <div class="header__adress">
        <img class="header__adress-img" src="./assets/images/drop.svg" alt="geo spot">
        <div class="header__adress-content">
          <div class="header__adress-item">г. Кишинев, ул. Бэнулеску Бодони, д. 33</div>
          <div class="header__adress-link">Мы на карте</div>
        </div>
      </div>
      <div class="header__phoneNumber">
        <span class="header__phoneNumber-item">069 82 77 38</span>
        <span class="header__phoneNumber-item">/</span>
        <span class="header__phoneNumber-item">079 92 77 38</span>
      </div>
      <img src="./assets/images/phone-call.svg" alt="phone call icon" class="header__phoneCall">
    </header>
    <section class="mainBanner center">
      <div id="circle1"></div>
      <div id="circle2"></div>
      <div id="circle3"></div>
      <div class="mainBanner__titler">
        <div class="mainBanner__title">Проблемы с Вашим устройством?</div>
        <div class="mainBanner__subtitle">Решаем любые проблемы!<br>Большой склад и опытные мастера</div>
        <div class="mainBanner__button">Бесплатная консультация</div>
      </div>
      <div class="mainBanner__elements">
        <img src="./assets/images/wave.svg" alt="waves" class="mainBanner__elements-waves">
        <img src="./assets/images/five-arrows.svg" alt="arrow" class="mainBanner__elements-arrow">
        <img src="./assets/images/ellipse.svg" alt="ellipse" class="mainBanner__elements-ellipse">
        <img src="./assets/images/dots.svg" alt="dots" class="mainBanner__elements-dots">
      </div>
      <div class="mainBanner__master">        
        <div class="mainBanner__master-monitor">
          <img src="./assets/images/circle3.svg" alt="monitor">
        </div>
        <div class="mainBanner__master-phone">
          <img src="./assets/images/circle4.svg" alt="phone">
        </div>
        <div class="mainBanner__master-gear">
          <img src="./assets/images/circle1.svg" alt="gear" id="gear-img">
        </div>
        <div class="mainBanner__master-laptop">
          <img src="./assets/images/circle2.svg" alt="laptop">
        </div>
        <div class="mainBanner__master-image">
          <div class="mainBanner__master-circle"></div>
          <div class="mainBanner__master-circle1"></div>
          <img src="./assets/images/master2.png" alt="master image">
        </div>
      </div>
      <div class="mainBanner__action">
        <div class="mainBanner__discount">
          <span class="mainBanner__discount-text">50%</span>
          <img src="./assets/images/fire.svg" class="mainBanner__discount-image" alt="fire image">
        </div>
        <div class="mainBanner__content">
          скидка на ремонт телефонов, ноутбуков и планшетов до <b>-50%</b>
        </div>
        <hr class="mainBanner__line">
        <div class="mainBanner__counter">
          <p class="mainBanner__counter-title">Конец акции:</p>
          <div class="mainBanner__counter-content">
          <div class="mainBanner__counter-item">
            <span class="item-value">2</span><br>
            <span class="item-title">DAYS</span>
          </div>
          <div class="mainBanner__counter-devider">:</div>
          <div class="mainBanner__counter-item">
            <span class="item-value">18</span><br>
            <span class="item-title">HOURS</span>
          </div>
          <div class="mainBanner__counter-devider">:</div>
          <div class="mainBanner__counter-item">
            <span class="item-value">56</span><br>
            <span class="item-title">MINUTES</span>
          </div>
        </div>
        </div>
      </div>
      <div class="mainBanner__advantages">
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/truck.svg" alt="truck image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Курьер по городу</div>
          <div class="mainBanner__advantages-content">Выезд курьера Буюканы Чеканы, Рышкановка, центр, Ботаника.</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/replace-phone.svg" alt="replace-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Подменный телефон - Бесплатно</div>
          <div class="mainBanner__advantages-content">Телефон взамен Беслатно, пока ваш в ремонте</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/adv-phone.svg" alt="adv-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Забота о вас</div>
          <div class="mainBanner__advantages-content">Незначительные поломки - делаем бесплатно.</div>
        </div>
      </div>


    </section>



    <section class="sec1 center">Lorem ipsum dolor sit amet.</section>
    <section class="sec1 center">Lorem ipsum dolor sit amet.</section>
    <section class="sec1 center">Lorem ipsum dolor sit amet.</section>

    <footer class="footer center">Lorem, ipsum dolor.</footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
  }
}
</script>

<style lang="scss">
#app {
  $widthSiteDesctop: 1920px;
  $commonBgColor: #f4f9fc;
  $mainTextColor: #13171D;
  $mainBannerSubtitleColor: #444444;
  $buttonTextColor: white;
  $buttonColor: #E2001A;
  $discountTextColor: #FF6b00;

  @mixin textDecoration ($fontFamily, $weight, $size, $lineH:normal, $letterSpacing:normal, $style:normal) {
      font-family: $fontFamily;
      font-weight: $weight;
      font-size: $size;
      line-height: $lineH;
      letter-spacing: $letterSpacing;
      font-style: $style;
  }

  @font-face {
        font-family: 'Gilroy';
        src: url('~@/assets/fonts/Gilroy/Gilroy-SemiBold.eot');
        src: local('Gilroy SemiBold'), local('Gilroy-SemiBold'),
              url('~@/assets/fonts/Gilroy/Gilroy-SemiBold.eot?#iefix') format('embedded-opentype'),
              url('~@/assets/fonts/Gilroy/Gilroy-SemiBold.woff') format('woff'),
              url('~@/assets/fonts/Gilroy/Gilroy-SemiBold.ttf') format('truetype');
        font-weight: 600;
        font-style: normal;
      }
  
  // a {
  //   text-decoration: none;
  // }

  .center {
    padding-left: calc(50% - $widthSiteDesctop / 2);
    padding-right: calc(50% - $widthSiteDesctop / 2);
  }

  .header {
    margin-top: 30px;
    margin-left: 30px;
    margin-right: 30px;
    display: flex;
    align-items: center;
    &__categories {
      @include textDecoration(Gilroy, 600, 16px, 19px, calc(1em * -0.01));
      color: $mainTextColor;
      padding-left: 78px;
      padding-right: 291px;
      display: flex;
      flex-direction: row;
      gap: 24px;
    }
    &__adress {      
      width: 330px;
      display: flex;
      flex-direction: row;
      gap: 16px;
      &-item{
        @include textDecoration(Montserrat, 400, 14px, 17px, calc(1em * -0.01));
      }
      &-link {
        @include textDecoration(Montserrat, 400, 12px, 15px, calc(1em * -0.01));
        color: blue;
        text-decoration: underline;
      }
      &-content {
        display: flex;
        flex-direction: column;
      }
    }
    &__phoneNumber {    
      width: 262px;
      padding-left: 45px;
      padding-right: 35px;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      &-item {
        @include textDecoration(Gilroy, 600, 20px, 24px, calc(1em * -0.01));
      }
    }
  }

  .mainBanner {
    margin-left: 74px;
    margin-right: 58px;
    height: 1118px;
    &__titler {
      width: 635px;
      height: 300px;
      position: absolute;
      // width: 625px;
      // height: 492px;
      left: 307.16px;
      right: 855.62px;
      top: 390.29px;
      bottom: 235.83px;
    }
    &__title {
      @include textDecoration("Bebas Neue", 700, 110px, 100px, calc(1em * -0.01));
      color: $mainTextColor;
    }
    &__subtitle {
      padding-top: 20px;
      padding-bottom: 40px;
      @include textDecoration(Gilroy, 400, 24px, 34px, calc(1em * -0.01));
      color: $mainBannerSubtitleColor;
    }
    &__button {
      width: 224px;
      height: 28px;
      @include textDecoration(Montserrat, 600, 16px, 26px, calc(1em * -0.01));
      color: $buttonTextColor;
      background: rgb(226,0,26);
      border-radius: 15px;
      padding: 18px 30px;
      outline: none;
      user-select: none;
    }
    &__button:hover {
      color: $buttonColor;
      border: 2px solid $buttonColor;
      background: rgb(255,255,255);
    }
    &__action {
      position: absolute;
      left: 1340.16px;
      right: 183.62px;
      top: 431.29px;
      bottom: 339.83px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      width: 204px;
      height: 309px;
      background-color: white;
      border-radius: 30px;
      // padding-top: -38px;
      padding-left: 30px;
      padding-right: 30px;
    }
    &__discount {
      margin-top: -38px;
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      gap: 21px;
      &-text {
        @include textDecoration('Bebas Neue', 700, 113px, 113px, calc(1em * -0.01));
        color: $discountTextColor;
      }
      &-image {
        width: 24px;
        height: 32px;
        margin-bottom: 20px;
      }
    }
    &__content {
      @include textDecoration(Gilroy, 400, 20px, 26px);
       color: $mainTextColor;
    }
    &__line {
      margin-top: 22px;
      margin-bottom: 22px;
      color: rgba(19, 23, 29, 0.5);
      width: 204px;
    }
    &__counter {
      &-title {
        margin: 0px;
        @include textDecoration(Gilroy, 600, 20px, 24px, calc(1em * -0.01));
        color: rgba(19, 23, 29, 0.5);
      }
      &-content {
        display: flex;
        flex-direction: row;
        gap: 6px;
      }
      &-item {
        width: 48px;
      }
      &-devider {
        @include textDecoration(Gilroy, 600, 32px, 38px, calc(1em * -0.01));
        color: $mainTextColor;
      }

    }
    &__elements {
      position: absolute;
      width: 1787.78px;
      height: 585.52px;
      left: 74px;
      right: -74px;
      top: 363.56px;
      bottom: 169.04px;
      &-waves {
        position: absolute;
        width: 98.3px;
        height: 62.01px;
        left: 92.43%;
        right: 2.07%;
        top: 62.09%;
        bottom: 27.32%;
      }
      &-arrow {
        position: absolute;
        width: 88.71px;
        height: 13.01px;
        left: 42.93%;
        right: 52.11%;
        top: 70.23%;
        bottom: 27.55%;
        // color: black;
        // opacity: 0.1;
      }
      &-dots {
        position: absolute;
        width: 56.4px;
        height: 56.38px;
        left: 100.98%;
        right: -4.14%;
        top: 148.6%;
        bottom: -58.23%;
      }
      &-ellipse {
        position: absolute;
        width: 50px;
        height: 50px;
        left: 74px;
        right: 1663.78px;
        top: 899.08px;
        bottom: -363.56px;
      }
    }
    &__master {
      position: absolute;
      width: 765px;
      height: 851.27px;
      left: 839.16px;
      right: 183.62px;
      top: 185.29px;
      bottom: 81.56px;
      &-image {
        position: absolute;
        // width: 765px;
        // height: 851.27px;
        // left: 839.16px;
        // right: -839.16px;
        // top: 185.29px;
        // bottom: -185.29px;
      }
      &-circle {
        position: absolute;
        border-radius: 247.55px;
        width: 495.09px;
        height: 495.09px;
        left: 974.16px;
        right: -704.24px;
        top: 406.48px;
        bottom: -50.29px;
        background: linear-gradient(180.00deg, rgb(0, 90, 170),rgb(61, 138, 255) 100%);
      }
      &-circle1 {
        position: absolute;
        width: 765px;
        height: 765px;
        border-radius: 382.5px;
        left: 839.16px;
        top: 271.56px;
        border: 1px dashed rgb(0, 0, 0);
        opacity: 0.3;
      }
      &-monitor {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 29.27px;
        width: 58.54px;
        height: 58.54px;
        left: 1434.66px;
        right: -1434.66px;
        top: 915.29px;
        bottom: -915.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
      }
      &-phone {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 36.27px;
        width: 72.54px;
        height: 72.54px;
        left: 840.89px;
        right: -840.89px;
        top: 778.29px;
        bottom: -778.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
      }
      &-gear {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 42.27px;
        width: 84.54px;
        height: 84.54px;
        left: 966.89px;
        right: -966.89px;
        top: 292.29px;
        bottom: -292.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
       
      }
      &-laptop {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 25.27px;
        width: 50.54px;
        height: 50.54px;
        left: 1425.66px;
        right: -1425.66px;
        top: 318.29px;
        bottom: -318.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);        
      }
    }
    &__advantages {
      position: absolute;
      width: 1298px;
      height: 192px;
      left: 352px;
      right: 137.78px;
      top: 1021px;
      bottom: -94.87px;
      display: flex;
      justify-content: space-between;
      &-item {
        width: 364px;
        display: flex;
        flex-direction: column;
      }
      &-image {
        width: 80px;
        height: 80px;
      }
      &-title {
        @include textDecoration(Gilroy, 600, 20px, 24px);
        color: $mainTextColor;
        margin-top: 24px;
        margin-bottom: 16px;
      }
      &-content {
        @include textDecoration(Gilroy, 400, 18px, 24px);
        color: $mainBannerSubtitleColor;
        // opacity: 0.5;
      }
    }

  }
  .item-value {
    text-align: center;
    @include textDecoration(Gilroy, 600, 32px, 38px, calc(1em * -0.01));
        color: $mainTextColor;
  }
  .item-title {
    @include textDecoration(Gilroy, 600, 11px, 13px, calc(1em * -0.01));
        color: rgba(19, 23, 29, 0.5);
  }
  #circle1 {
    position: absolute;
    border-radius: 528px;
    width: 1056px;
    height: 1056px;
    left: 724.16px;
    right: 7.62px;
    top: 96.29px;
    bottom: -34.17px;
    border-radius: 500px;
    filter: blur(200px);
    background: radial-gradient(50.00% 50.00% at 50% 50%,rgb(255, 107, 0),rgba(255, 107, 0, 0) 100%);
    opacity: 0.2;
  }
  #circle2 {
    position: absolute;
    width: 182px;
    height: 182px;
    border-radius: 91px;
    left: 243.16px;
    right: 1362.62px;
    top: 330.29px;
    bottom: 605.83px;
    background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
  }
  #circle3 {
    position: absolute;
    width: 1117px;
    height: 1118.13px;
    border-radius: 559px;
    left: 663.16px;
    right: 7.62px;
    top: 95px;
    bottom: -95px;
    background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
    opacity: 0.6;
  }
  #gear-img {
    opacity: 0.1;
  }
}
</style>
