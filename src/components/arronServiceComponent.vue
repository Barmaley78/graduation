<template>
        <section class="arronService center">
      <div class="arronService__vector"></div>
      <img src="../assets/images/ellipse.svg" alt="check list icon" class="arronService__vector1">
      <img src="../assets/images/dots.svg" alt="check list icon" class="arronService__vector2">
      <div class="arronService__content">
        <div class="arronService__left">
          <p class="arronService__title">что делать если ноутбук или телефон медленно работает</p>
          <div class="arronService__solution">
            <img src="../assets/images/check_list_icon.svg" alt="check list icon" class="arronService__icon">
            <p class="arronService__text">Получите чек лист - Что делать, если ноутбук или телефон грузится</p>
          </div>          
          <div class="arronService__button">Получить чек лист</div>          
        </div>
        <div class="arronService__right">
          <div class="arronService__right-item">
            <p class="arronService__title">Наши услуги</p>
            <ul class="arronService__list">
              <li>ремонт ноутбуков</li>
              <li>ремонт смартфонов</li>
              <li>заправка и ремонт картриджей</li>
              <li>установка СНПЧ</li>
              <li>ремонт компьютеров</li>
              <li>ремонт моноблоков</li>
            </ul>
          </div>
          <div class="arronService__right-item">
            <ul class="arronService__list">
              <li>ремонт планшетов</li>
              <li>ремонт КПК</li>
              <li>ремонт принтеров</li>
              <li>ремонт роутеров</li>
              <li>всстановление жестких дисков</li>
              <li>компьютерная помощь и IT аутсорсинг и др.</li>
            </ul>
          </div>       
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'arronServiceComponent'
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
            font-weight: 600;
            font-style: normal;
    }

    .center {
        padding-left: calc(50% - $widthSiteDesctop / 2);
        padding-right: calc(50% - $widthSiteDesctop / 2);
    }

    .arronService {
        position: relative;
        margin: 0 auto;
        width: 1476px;
        margin-top: -65px;
        padding-top: 160px;
        padding-bottom: 64px;
        &__content {
            padding-left: 126px;
            padding-right: 134px;
            display: flex;
            flex-direction: row;
            gap: 125px;
            align-items: center;
        }
        &__left {
            max-width: 427px;
            display: flex;
            flex-direction: column;
        }
        &__title {
            text-transform: uppercase;
            margin: 0 0;
            @include textDecoration("Babes Neue", 700, 48px, 48px, calc(1em * -0.3));
            color: $mainTextColor;
        }
        &__icon {
            width: 35px;
            height: 45px;
        }
        &__text {
            @include textDecoration(Montserrat, 400, 14px, 17x);
            color: black;
        }
        &__solution {
            width: 333px;
            padding-top: 6px;
            padding-bottom: 32px;
            display: flex;
            flex-direction: row;
            align-items: center;
            gap: 10px;
        }
        &__button {
            text-align: center;
            padding: 29px 35px 24px;
            width: 260px;
            height: 28px;
            border-radius: 15px;
            background: $buttonColor;
            @include textDecoration(Montserrat, 600, 16px, 26px);
            color: $buttonTextColor;
        }
        &__right {
            display: flex;
            flex-direction: row;
            gap: 32px;
            align-items: center;
            &-item{
                display: inline-block;
            }
        }
        &__list li {
            padding-bottom: 18px;
            @include textDecoration(Montserrat, 400, 18px, 24px);
            color: $mainBannerSubtitleColor;
        }
        &__list li::marker {
            color: $buttonColor;
            font-size: 24px;
        }
        &__vector {
            position: absolute;
            width: 276px;
            height: 276px;
            left: 0px;
            top: 0px;      
            background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
            border-radius: 50%;
        }
        &__vector2 {
            position: absolute;
            left: 1294px;
            top: 69px;
        }
        &__vector1 {
            position: absolute;
            left: 1426px;
            top: 490px;
        }
    }
</style>
