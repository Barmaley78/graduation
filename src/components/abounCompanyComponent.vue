<template>
        <section class="aboutCompany center">
      <div class="aboutCompany__left">
        <img src="../assets/images/grey-arrows.svg" alt="grey arrows image" class="aboutCompany__vector">
        <div class="aboutCompany__title">О компании Arron</div>
        <div class="aboutCompany__subtitle">Узнайте больше о нашей компании из видео за 1 минуту.</div>
        <div class="aboutCompany__button">
          <p class="aboutCompany__button-name">Смотреть</p>
          <img src="../assets/images/play-white.svg" alt="play image" class="aboutCompany__button-img">
        </div>
      </div>
      <div class="aboutCompany__right">
        <div class="aboutCompany__right-card">
          <img src="../assets/images/truck.svg" alt="truck image">
          <p class="aboutCompany__right-cardTitle">Выезжаем в любую точку Кишинева</p>
          <p class="aboutCompany__right-cardText">Выезд курьера Буюканы, Чеканы,<br>Рышкановка, центр, Ботаника.</p>          
        </div>
        <div class="aboutCompany__right-card">
          <img src="../assets/images/clock.svg" alt="clock image">
          <p class="aboutCompany__right-cardTitle">Работы от 30 минут</p>
          <p class="aboutCompany__right-cardText">Время работы или настройки занимает<br>от 30 минут до нескольких часов.</p>    
        </div>
        <div class="aboutCompany__right-card">
          <img src="../assets/images/money.svg" alt="money image">
          <p class="aboutCompany__right-cardTitle">Удобный способ оплаты</p>
          <p class="aboutCompany__right-cardText">Оплата наличными или по<br>перечислению компаниям.</p>    
        </div>
        <div class="aboutCompany__right-card">
          <img src="../assets/images/shild.svg" alt="shild image">
          <p class="aboutCompany__right-cardTitle">Гарантия на все выполненные услуги</p>
          <p class="aboutCompany__right-cardText">Запчасти, фотографии и сообщения<br>под Вашим контролем. После работ<br>инженер отдаст Вам старые запчасти.</p>    
        </div>
      </div>
      <img src="../assets/images/wave.svg" alt="wave image" class="aboutCompany__wave">
    </section>    
</template>

<script>
export default {
  name: 'abounCompanyComponent'
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
    .aboutCompany {
        position: relative;
        display: flex;
        flex-direction: row;
        gap: 110px;
        height: 545px;
        // width: 1298px;
        margin: 0 auto;
        background: linear-gradient(180.00deg, rgb(235, 243, 248),rgba(235, 243, 248, 0) 100%);
        &__left {
            position: relative;
            padding-left: 311px;
            padding-top: 80px;
            width: 333px;
            height: 402px;
            display: flex;
            flex-direction: column;
        }
        &__title {
            text-transform: uppercase;
            @include textDecoration("Babes Neue", 700, 80px, 80px, calc(1em * -0.35));
            color: $mainTextColor;
        }
        &__subtitle {
            padding-top: 24px;
            padding-bottom: 64px;
            @include textDecoration(Gilroy, 400, 24px, 30px);
            color: $mainBannerSubtitleColor;
        }
        &__vector {
            position: absolute;
            left: 537px;
            top: 186px;
        }
        &__button {
            display: flex;
            flex-direction: row;
            align-items: center;
            gap: 16px;
            padding: 18px 30px;
            width: 122px;
            height: 28px;
            border-radius: 15px;
            background: rgb(226, 0, 26);
            &-name {
                @include textDecoration(Montserrat, 600, 16px, 26px);
                color: $buttonTextColor;
            }
            &-img {
                width: 14px;
                height: 18px;
            }
        }
        &__right {
            padding-top: 97px;
            width: 788px;
            margin-right: 75px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr;
            row-gap: 40px;
            column-gap: 80px;
            &-card {
                display: inline-block;
            }
            &-cardTitle {
                @include textDecoration(Gilroy, 600, 20px, 24px);
                color: $mainTextColor;
            }
            &-cardText {
                @include textDecoration(Gilroy, 400, 18px, 24px);
                color: $mainBannerSubtitleColor;
            }
        }
        &__wave {
            position: absolute;
            left: 1645px;
            top: 417px;
            width: 98px;
        }
  }
</style>
