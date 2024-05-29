<template>
    <section class="mainBanner center">
      <div class="mainBanner__block">
        <div id="circle1"></div>
        <div id="circle2"></div>
        <div id="circle3"></div>
        <div class="mainBanner__master">        
          <div class="mainBanner__master-circle"></div>
          <div class="mainBanner__master-circle1"></div>
          <div class="mainBanner__master-monitor">
            <img src="../assets/images/circle3.svg" alt="monitor">
          </div>
          <div class="mainBanner__master-phone">
            <img src="../assets/images/circle4.svg" alt="phone">
          </div>
          <div class="mainBanner__master-gear">
            <img src="../assets/images/circle1.svg" alt="gear" id="gear-img">
          </div>
          <div class="mainBanner__master-laptop">
            <img src="../assets/images/circle2.svg" alt="laptop">
          </div>
          <img src="../assets/images/master-vector.svg" alt="vector element" class="mainBanner__master-vector">
          <img src="../assets/images/master2.png" alt="master image" class="mainBanner__master-image">
        </div>
        <div class="mainBanner__title">
          <div class="mainBanner__name">Проблемы<br>с Вашим<br>устройством?</div>
          <div class="mainBanner__subtitle">Решаем любые проблемы!<br>Большой склад и опытные мастера</div>
          <div class="mainBanner__button">Бесплатная консультация</div>
        </div>
        <div class="mainBanner__action">
          <div class="mainBanner__discount">
            <span class="mainBanner__discount-text">50%</span>
            <img src="../assets/images/fire.svg" class="mainBanner__discount-image" alt="fire image">
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
      </div>
      <div class="mainBanner__elements">
        <img src="../assets/images/wave.svg" alt="waves" class="mainBanner__elements-waves">
        <img src="../assets/images/grey-arrows.svg" alt="arrow" class="mainBanner__elements-arrow">
        <img src="../assets/images/ellipse.svg" alt="ellipse" class="mainBanner__elements-ellipse">
        <img src="../assets/images/dots.svg" alt="dots" class="mainBanner__elements-dots">
      </div>
      <div class="mainBanner__advantages">
        <div class="mainBanner__advantages-item">
          <img src="../assets/images/truck.svg" alt="truck image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Курьер по городу</div>
          <div class="mainBanner__advantages-content">Выезд курьера Буюканы Чеканы, Рышкановка, центр, Ботаника.</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="../assets/images/replace-phone.svg" alt="replace-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Подменный телефон - Бесплатно</div>
          <div class="mainBanner__advantages-content">Телефон взамен Беслатно, пока ваш в ремонте</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="../assets/images/adv-phone.svg" alt="adv-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Забота о вас</div>
          <div class="mainBanner__advantages-content">Незначительные поломки - делаем бесплатно.</div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'mainBannerComponent'
}
</script>

<style scoped lang="scss">
    $widthSiteDesctop: 1920px;
    $widthMainBlockDesctop: 1300px;
    $commonBgColor: #f4f9fc;
    $mainTextColor: #13171D;
    $mainBannerSubtitleColor: #444444;
    $buttonTextColor: white;
    $buttonColor: #E2001A;
    $discountTextColor: #FF6b00;
    $aboutTextColor: #646464;

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
            // font-weight: 600;
            // font-style: normal;
    }

    @font-face {
    font-family: 'Bebas Neue';
    src: url('~@/assets/fonts/BebasNeue/BebasNeueRegular.eot');
    src: local('Bebas Neue Regular'), local('BebasNeueRegular'),
        url('~@/assets/fonts/BebasNeue/BebasNeueRegular.eot?#iefix') format('embedded-opentype'),
        url('~@/assets/fonts/BebasNeue/BebasNeueRegular.woff2') format('woff2'),
        url('~@/assets/fonts/BebasNeue/BebasNeueRegular.woff') format('woff'),
        url('~@/assets/fonts/BebasNeue/BebasNeueRegular.ttf') format('truetype');
    // font-weight: normal;
    // font-style: normal;
  }

    .center {
        padding-left: calc(50% - $widthSiteDesctop / 2);
        padding-right: calc(50% - $widthSiteDesctop / 2);
    }

    .mainBanner {
      position: relative;
      margin-left: 74px;
      margin-right: 58px;
      height: 1118px;
      width: 1788px;
      &__title {
        width: 635px;     
        position: absolute;
        left: 277px;
        top: 295px;
      }
      &__name {
        @include textDecoration("Bebas Neue", 700, 100px, 100px, calc(1em * -0.01));
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
      &__block{
        position: relative;
      }
      &__master {
        position: absolute;
        left: -3px;
        top: -42px;
        &-vector {
          position: absolute;
          left: 1287.7px;
          top: 206.7px;
          border: 1px solid rgb(19, 23, 29);
          visibility: hidden;
        }
        &-image {
          position: absolute;
          left: 965px;
          top: 239px;
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
          border: 2px dashed rgb(0, 0, 0);
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
      &__elements {
        position: relative;
        width: 1788px;
        height: 585.5px;
        top: 363.6px;
        &-waves {
          position: absolute;
          left: 1586.5px;
          top: 0px;
        }
        &-arrow {
          position: absolute;
          left: 701.5px;
          top: 47.6px;
        }
        &-dots {
          position: absolute;
          right: -54.6px;
          top: 506.5px;
        }
        &-ellipse {
          position: absolute;
          left: 0px;
          top: 535.5px;
        }
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
        @include textDecoration(Gilroy, 400, 18px, 26px);
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
      &__advantages {
        position: relative;
        width: 1298px;
        height: 192px;
        left: 311px;
        top: 400px;
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

    #gear-img {
      opacity: 0.1;
    }

    #circle1 {
          position: absolute;
          border-radius: 50%;
          width: 1056px;
          height: 1056px;
          left: 724.16px;
          top: 0px;
          filter: blur(200px);
          background: radial-gradient(50.00% 50.00% at 50% 50%,rgb(255, 107, 0),rgba(255, 107, 0, 0) 100%);
          opacity: 0.2;
    }
    #circle2 {
        position: absolute;
        width: 182px;
        height: 182px;
        border-radius: 50%;
        left: 177px;
        top: 234px;
        background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
    }
    #circle3 {
        position: absolute;
        width: 1118px;
        height: 1118px;
        border-radius: 50%;
        left: 597px;
        top: 0px;
        background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
        opacity: 0.6;
    }
</style>
