<template>
       <section class="about center">
      <img src="../assets/images/wave-blue.svg" alt="wave image" class="about__vector1">
      <img src="../assets/images/grey-arrows.svg" alt="wave image" class="about__vector2">
      <img src="../assets/images/ellipse.svg" alt="wave image" class="about__vector3">
      <div class="about__header">
        <img src="../assets/images/quotation.svg" alt="" class="about__header-el1">
        <div class="about__header-el2">
          В нашей компании работают лучшие специалисты, которые прекрасно разбираются 
          в современных технологиях и имеют более 3-х лет опыта работы.
        </div>
        <img src="../assets/images/quotation.svg" alt="" class="about__header-el3">
      </div>
      
      <div class="about__content">
        <div class="about__content-left">
          <p class="about__content-text">
            За счет этого мы гарантируем устранение любых неполадок и 
            предоставляем гарантию на все выполненные работы.
          </p>
          <p class="about__content-text">
            Мы поможем не только восстановить работоспособность техники, но и подскажем, 
            как избежать возникновения подобных поломок в будущем.
          </p>
          <p class="about__content-text">
            Квалифицированная консультация специалиста поможет безопасно пользоваться 
            компьютером. В нашем штате работают опытные специалисты.
          </p>
        </div>
        <div class="about__content-right">
          <div class="about__content-buttons">
            <img src="../assets/images/master3.jpg" alt="about master image" class="about__content-img">

            <div class="about__content-backward">
              <div class="about__content-circle1"></div>
              <div class="about__content-circle2"></div>
              <img src="../assets/images/chevron-left.svg" alt="" class="about__content-arrow">
            </div>

            <div class="about__content-forward">
              <div class="about__content-circle1"></div>
              <div class="about__content-circle2"></div>
              <img src="../assets/images/chevron-right.svg" alt="" class="about__content-arrow">
            </div>
          </div>  

          <div class="carousel__nav">
            <div class="carousel__nav-item" id="checked"></div> 
            <div class="carousel__nav-item"></div> 
            <div class="carousel__nav-item"></div> 
            <div class="carousel__nav-item"></div> 
            <div class="carousel__nav-item"></div> 
          </div>
        </div>
      </div>


    </section> 
</template>

<script>
export default {
  name: 'aboutComponent'
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

    .buttonCircle {
        width: 48px;
        height: 48px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        border-radius: 23px;
        box-shadow: 0px 8px 16px 0px rgba(255, 107, 0, 0.16);
        background: rgb(255, 255, 255);
    }

    .carousel {
        &__buttons {
            display: flex;
            flex-direction: row;
            gap: 16px;
        }
        &__nav {
            width: 112px;
            height: 16px;
            display: grid;
            grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
            column-gap: 8px;
            &-item {
                width: 4px;
                height: 4px;
                background: $mainTextColor;
                box-sizing: border-box;
                padding: 6px;
                border-radius: 50%;
                opacity: 0.5;
            }
            &-item#checked {
                width: 8px;
                height: 8px;
                background: $commonBgColor;
                box-sizing: border-box;
                border: 4px solid $buttonColor;
                border-radius: 50%;
                opacity: 1;
            }
        }
    }

    .about {
        margin: 0 auto;
        padding-bottom: 84px;
        width: $widthMainBlockDesctop;
        position: relative;
        &__vector1 {
            position: absolute;
            left: -94px;
            top: 136px;
        }
        &__vector2 {
            position: absolute;
            left: 456px;
            top: 362px;
        }
        &__vector3 {
            width: 73px;
            height: 73px;
            z-index: -1;
            position: absolute;
            left: 1157px;
            top: 635px;
        }
        &__header {
            margin: 0 auto;
            width: 740px;
            padding-bottom: 56px;
            &-el1 {}
            &-el2 {
                @include textDecoration(Montserrat, 500, 24px, 32px);
                text-align: center;
                color: $mainTextColor;
            }
            &-el3 {
                transform: scale(-1, 1);
                float: right;
            }
        }
        &__content {
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
            &-left {
                width: 470px;
            }
            &-text {
                @include textDecoration(Montserrat, 400, 18px, 24px);
                color: $aboutTextColor;
            }
            &-right {
                width: 635px;
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 20px;
            }
            &-img {
                border-radius: 20px;
            }
            &-buttons {
                width: 715px;
                display: flex;
            }
            &-backward {
                display: flex;
                align-content: center;
                justify-content: center;
                align-items: center;
                flex-direction: row;
            }
            &-forward {
                display: flex;
                align-content: center;
                justify-content: center;
                align-items: center;
                flex-direction: row;
            }
            &-circle1 {
                width: 80px;
                height: 80px;
                background: rgb(250, 252, 254);
                border-radius: 50%;
            }
            &-circle2 {
                width: 48px;
                height: 48px;
                border-radius: 50%;
                box-shadow: 0px 8px 16px 0px rgba(255, 107, 0, 0.16);
                background: rgb(255, 255, 255);
            }
            &-arrow {
                width: 24px;
                height: 24px;
            }
        }
    }
</style>
