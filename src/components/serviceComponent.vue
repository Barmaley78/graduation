<template>
    <section class="service center">
      <div class="span-col">
        <div class="service-circle"></div>
        <div class="service__title">Мы работаем <br> с устройствами:</div>
      </div>
      <div class="service__item" id="apple">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/dots_45.svg" alt="dots" class="service__item-vector">
        <img src="../assets/images/apple.png" alt="apple image" class="service__item-img">
        <div class="service__item-logoCircle"></div>
        <img src="../assets/images/apple-logo.svg" alt="apple logo image" class="service__item-logo">      
        <div class="service__item-title">Apple</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="android">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/wave.svg" alt="waves" class="service__item-vector">
        <img src="../assets/images/android.png" alt="android image" class="service__item-img">
        <div class="service__item-logoCircle"></div>
        <img src="../assets/images/android-logo.svg" alt="android logo image" class="service__item-logo">      
        <div class="service__item-title">Android</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="gadgets">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/wave.svg" alt="waves" class="service__item-vector">
        <img src="../assets/images/gadgets.png" alt="gadgets image" class="service__item-img">
        <div class="service__item-title">Гаджетами</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="laptop">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/triangle.svg" alt="triangle" class="service__item-vector">
        <img src="../assets/images/laptop.png" alt="laptop image" class="service__item-img">
        <div class="service__item-title">Ноутбуками</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="pc">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/yellow-arrows.svg" alt="yellow-arrows" class="service__item-vector">
        <img src="../assets/images/pc.png" alt="pc image" class="service__item-img">
        <div class="service__item-title">Моноблоками и РС</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>
      
      <div class="service__item" id="devices">
        <div class="service__item-rectangle"></div>
        <img src="../assets/images/grey_triangle.svg" alt="grey_triangle" class="service__item-vector">
        <img src="../assets/images/devices.png" alt="devices image" class="service__item-img">
        <div class="service__item-title">Другими устройствами</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="../assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>
    </section>    
</template>

<script>
export default {
  name: 'serviceComponent'
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
    .service {
        margin: 0 auto;
        padding-top: 240px;
        padding-bottom: 80px;
        width: 1298px;
        height: 770px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        row-gap: 10px;
        column-gap: 30px;
        &__title {
            position: absolute;
            text-transform: uppercase;
            top: 106px;
            @include textDecoration("Bebas Neue", 700, 80px, 84px);
            color: $mainTextColor;
        }
        &__item {      
            width: 302px;
            height: 390px;
            position: relative;
            &-title {        
                position: absolute;
                left:30px;
                top: 259px;
                @include textDecoration(Gilroy, 600, 22px, 30px);
                color: $mainTextColor;
            }
            &-vector {
                position: absolute;
                top: 58.3px;
                left: 14.4px;
            }
            &-img {        
                // width: 183px;
                // height: 241px;
                position: absolute;
                left: 35px;
            }    
            &-logo {
                // width: 32.58px;
                // height: 40px;
                position: absolute;
                top: 137px;
                left: 201px;
            }
            &-logoCircle{
                width: 92px;
                height: 92px;
                position: absolute;
                top: 111px;
                left: 171px;
                box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
                background: rgb(255, 255, 255);
                border-radius: 50%;
            }
            &-arrow {        
                width: 24px;
                height: 24px;
                position: absolute;
                top: 317px;
                left: 238px;
            }
            &-rectangle {        
                width: 302px;
                height: 310px;
                position: absolute;
                top: 30px;
                border-radius: 30px;
                clip-path: polygon(0% 15%, 100% 0%, 100% 100%, 0% 90%);
                box-shadow: 0px 8px 10px 0px rgba(255, 107, 0, 0.08),0px 50px 60px 0px rgba(255, 107, 0, 0.08);
                background: rgb(255, 255, 255);
                opacity: 0.5;
            }
        }
    }
    .span-col {
        position: relative;
        grid-column: auto / span 2;
    }

    .service-circle {    
        width: 182px;
        height: 182px;
        border-radius: 50%;
        position: absolute;
        left: 231px;
        top: 113px;
        transform: rotate(30.00deg);
        background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
        opacity: 0.8;
    }
    .arrow-circle1 {    
        width: 40px;
        height: 40px;
        position: absolute;
        top: 308px;
        left: 230px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
        border-radius: 50%;
    }
    .arrow-circle2 {    
        width: 64px;
        height: 64px;
        position: absolute;
        top: 296px;
        left: 218px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
        border-radius: 50%;
    }
</style>
