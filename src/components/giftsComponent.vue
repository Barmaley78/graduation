<template>
    <section class="gifts center">
      <div class="gifts__content">        
        <div class="gifts__header">
          <div class="gifts__circle"></div>
          <div class="gifts__title">На каждый ремонт гарантировано подарок на ваш выбор :</div>
          <div class="carousel__buttons">
            <div class="buttonCircle">
              <img src="../assets/images/chevron-left.svg" alt="left button arrow" class="buttonCircle-left">
            </div>
            <div class="buttonCircle">
              <img src="../assets/images/chevron-right.svg" alt="right bbuttonCircleutton arrow" class="buttonCircle-right">
            </div>
          </div>
        </div>
        <div class="gifts__cards">
          <div class="gifts__cards-item">
            <div class="gifts__cards-rect"></div>
            <img src="../assets/images/wave.svg" alt="" class="gifts__cards-vector1">
            <img src="../assets/images/ellipse-grey.svg" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift1.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Чехлы</p>
          </div>

          <div class="gifts__cards-item">
            <div class="gifts__cards-rect"></div>
            <img src="../assets/images/triangle.svg" alt="" class="gifts__cards-vector1">
            <img src="../assets/images/ellipse.svg" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift2.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Защитные стекла</p>
          </div>

          <div class="gifts__cards-item">
            <div class="gifts__cards-rect"></div>
            <img src="../assets/images/yellow-arrows.svg" alt="" class="gifts__cards-vector1">
            <img src="../assets/images/polygon2.svg" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift3.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Кабели</p>
          </div>

          <div class="gifts__cards-item">
            <div class="gifts__cards-rect"></div>
            <img src="" alt="" class="gifts__cards-vector1">
            <img src="../assets/images/wave.svg" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift4.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Car holder</p>
          </div>

          <div class="gifts__cards-item" id="hidden">
            <div class="gifts__cards-rect"></div>
            <img src="" alt="" class="gifts__cards-vector1">
            <img src="" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift5.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Зарядки</p>
          </div>

          <div class="gifts__cards-item" id="hidden">
            <div class="gifts__cards-rect"></div>
            <img src="" alt="" class="gifts__cards-vector1">
            <img src="" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift6.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Наушники</p>
          </div>

          <div class="gifts__cards-item" id="hidden">
            <div class="gifts__cards-rect"></div>
            <img src="" alt="" class="gifts__cards-vector1">
            <img src="" alt="" class="gifts__cards-vector2">
            <img src="../assets/images/gift7.png" alt="" class="gifts__cards-img">
            <p class="gifts__cards-name">Другие аксесуары</p>
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
  name: 'giftsComponent'
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
    .gifts {
        margin: 0 auto;
        background: linear-gradient(180.00deg, rgb(235, 243, 248),rgba(235, 243, 248, 0) 100%);
        padding-bottom: 145px;
        &__circle {
            z-index: -1;
            position: absolute;
            width: 182px;
            height: 182px;
            left: 321px;
            top: 150px;
            transform: rotate(30.00deg);
            background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
            opacity: 0.8;
            border-radius: 50%;
        }
        &__content {
            width: $widthMainBlockDesctop;
            margin: 0 auto;
        }
        &__title {
            padding-top: 133px;
            padding-right: 200px;
            padding-bottom: 63px;
            text-transform: uppercase;
            @include textDecoration("Bebas Neue", 700, 80px, 84px);
        color: $mainTextColor;
        }
        &__header {
            position: relative;
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: flex-end;
        }
        &__cards {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr 1fr;
            column-gap: 31px;
            &-item {
                display: block;
                width: 302px;
                height: 310px;
                position: relative;
            }
            &-item#hidden {
                display: none;
            }
            &-rect {
                width: 302px;
                height: 310px;
                position: absolute;
                left: 0px;
                top: 0px;
                clip-path: polygon(0% 15%, 100% 0%, 100% 100%, 0% 90%);
                border-radius: 30px;        
                box-shadow: 0px 8px 10px 0px rgba(255, 107, 0, 0.08),0px 50px 60px 0px rgba(255, 107, 0, 0.08);
                background: rgb(255, 255, 255);
                opacity: 0.5;
            }
            &-img {
                position: absolute;
            }
            &-vector1 {
                position: absolute;
                left: 5px;
                top: 20px;
            }
            &-vector2 {
                position: absolute;
                left: 200px;
                top: 120px;
            }
            &-name {
                position: absolute;
                left: 30px;
                top: 220px;
                @include textDecoration(Gilroy, 600, 22px, 30px);
                color: $mainTextColor;
            }
        }
    }
</style>
