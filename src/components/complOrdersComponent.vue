<template>
    <section class="complOrders center">
      <div class="complOrders__block">
        <img src="../assets/images/wave.svg" alt="wawes image" class="complOrders__vector1">
        <img src="../assets/images/grey-arrows.svg" alt="arrows image" class="complOrders__vector2">
      </div>
      <div class="complOrders__cont">
        <div class="complOrders__header">
          <div class="complOrders__title">Выполненные заказы</div>
          <div class="carousel__buttons">
            <div class="buttonCircle">
              <img src="../assets/images/chevron-left.svg" alt="left button arrow" class="buttonCircle-left">
            </div>
            <div class="buttonCircle">
              <img src="../assets/images/chevron-right.svg" alt="right bbuttonCircleutton arrow" class="buttonCircle-right">
            </div>
          </div>
        </div>
        <div class="complOrders__content">
          <div class="complOrders__content-item">
            <img src="../assets/images/order1.jpg" alt="complOrders snap image" class="complOrders__img">
          </div>
          <div class="complOrders__content-item">
            <img src="../assets/images/order2.jpg" alt="complOrders snap image" class="complOrders__img">
          </div>
          <div class="complOrders__content-item">
            <img src="../assets/images/order3.jpg" alt="complOrders snap image" class="complOrders__img">
          </div>
        </div>
        <div class="carousel__nav">
        <div class="carousel__nav-item">
          <div class="carousel__nav-itemMark" id="checked"></div>
        </div> 
        <div class="carousel__nav-item">
          <div class="carousel__nav-itemMark"></div>
        </div> 
        <div class="carousel__nav-item">
          <div class="carousel__nav-itemMark"></div>
        </div> 
        <div class="carousel__nav-item">
          <div class="carousel__nav-itemMark"></div>
        </div> 
        <div class="carousel__nav-item">
          <div class="carousel__nav-itemMark"></div>
        </div> 
      </div>

    </div>
    </section> 
</template>

<script>
export default {
  name: 'complOrdersComponent'
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
            position: relative;
            margin: 0 auto;
            width: 112px;
            height: 16px;
            display: flex;
            
            gap: 8px;
            &-item {
                width: 16px;
                height: 16px;
            }
            &-itemMark{
                position: relative;
                left: 6px;
                top: 6px;
                width: 4px;
                height: 4px;
                background: $mainTextColor;
                box-sizing: border-box;
                border-radius: 50%;
                opacity: 0.5;
            }
            &-itemMark#checked {
                position: relative;
                left: 3px;
                top: 3px;
                width: 10px;
                height: 10px;
                background: $commonBgColor;
                box-sizing: border-box;
                border: 1px solid $buttonColor;
                border-radius: 50%;
                opacity: 1;
            }
        }
    }

    .complOrders {
        background: linear-gradient(180.00deg, rgb(235, 243, 248),rgba(235, 243, 248, 0) 100%);
        &__block {
          width: $widthMainBlockDesctop;
          margin: 0 auto;
          position: relative;
        }
        &__vector1 {
          z-index: -1;
          position: absolute;
          left: -68px;
          top: 523px;
        }
        &__vector2 {
          position: absolute;
          left: 505px;
          top: 98px;
        }
        &__cont {
            padding-top: 81px;            
            width: $widthMainBlockDesctop;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-content: space-between;
            gap: 48px;
        }
        &__header {
            display: flex;
            flex-direction: row;
            justify-content: space-between;
        }
        &__title {
            text-transform: uppercase;
            @include textDecoration("Bebas Neue", 700, 56px, 56px);
            color: $mainTextColor;
        }
        &__content{
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            column-gap: 32px;
            &-item {
                width: 412px;
                height: 400px;
            }
        }
        &__img {
            border-radius: 15px;
        }
    }
</style>
