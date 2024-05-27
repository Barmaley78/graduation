<template>
        <section class="feedback center">
      <img src="../assets/images/ellipse.svg" alt="ellipse image" class="feedback__vector1">
      <img src="../assets/images/dots.svg" alt="dots image" class="feedback__vector2">
      <div class="feedback__header">
        <div class="feedback__title">Отзывы счастливых клиентов</div>
        <div class="carousel__buttons">
          <div class="buttonCircle">
            <img src="../assets/images/chevron-left.svg" alt="left button arrow" class="buttonCircle-left">
          </div>
          <div class="buttonCircle">
            <img src="../assets/images/chevron-right.svg" alt="right bbuttonCircleutton arrow" class="buttonCircle-right">
          </div>
        </div>
      </div>

      <div class="feedback__content">
        <div class="feedback__content-item">
          <img src="../assets/images/feedback_1.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="../assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="../assets/images/feedback_2.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="../assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="../assets/images/feedback_3.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="../assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="../assets/images/feedback_4.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="../assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
      </div>

      <div class="carousel__nav">
        <div class="carousel__nav-item" id="checked"></div> 
        <div class="carousel__nav-item"></div> 
        <div class="carousel__nav-item"></div> 
        <div class="carousel__nav-item"></div> 
        <div class="carousel__nav-item"></div> 
      </div>

    </section>
</template>

<script>
export default {
  name: 'Component'
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

    .feedback {
            margin: 0 auto;
            padding-top: 120px;
            padding-bottom: 120px;
            width: $widthMainBlockDesctop;
            height: 420px;
            position: relative;
            display: flex;
            flex-direction: column;
            gap: 48px;
            &__header {
                display: flex;
                flex-direction: row;
                justify-content: space-between;
            }
            &__title {
                text-transform: uppercase;
                @include textDecoration("Babes Neue", 700, 56px, 56x, calc(1em * -0.35));
                color: $mainTextColor;
            }
            &__content{
                display: grid;
                grid-template-columns: 1fr 1fr 1fr 1fr;
                column-gap: 30px;
                // place-items: center;
                &-item {
                    width: 302px;
                    height: 250px;
                    display: flex;
                    flex-direction: row;
                    justify-content: center;
                    align-items: center;
                }
            }
            &__btn {
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                &-circle1 {
                    width: 72px;
                    height: 72px;
                    box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
                    background: rgb(255, 255, 255);
                    border-radius: 50%;
                    opacity: 0.5;
                }
                &-circle2 {
                    width: 56px;
                    height: 56px;
                    box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
                    background: rgb(255, 255, 255);
                    border-radius: 50%;
                }
                &-play {
                    width: 10.5px;
                    height: 13.5px;
                }
            }
            &__img {
                border-radius: 15px;
            }
            &__vector1 {
                position: absolute;
                left: -211px;
                top: 287px;
            }
            &__vector2 {
                position: absolute;
                left: 1488px;
                top: 258px;
            }
    }
</style>
