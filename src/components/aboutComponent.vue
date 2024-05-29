<template>
       <section class="about center">
        <div class="about__block">
            <img src="../assets/images/wave-blue.svg" alt="wave image" class="about__vector1">
            <img src="../assets/images/grey-arrows.svg" alt="arrows image" class="about__vector2">
            <img src="../assets/images/ellipse.svg" alt="ellipse image" class="about__vector3">
        </div>
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
            <div class="about__content-image">
                <img src="../assets/images/master3.jpg" alt="about master image" class="about__content-img">
                <div class="about__content-buttons">
                    <div class="about__content-backward">
                        <div class="about__content-circle1">
                            <div class="about__content-circle2">
                                <img src="../assets/images/chevron-left.svg" alt="" class="about__content-arrow">
                            </div>                    
                        </div>                    
                    </div>
                    <div class="about__content-forward">
                        <div class="about__content-circle1">
                            <div class="about__content-circle2">
                                <img src="../assets/images/chevron-right.svg" alt="" class="about__content-arrow">
                            </div>                    
                        </div>                    
                    </div>
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

    .about {
        margin: 0 auto;
        padding-bottom: 84px;
        width: $widthMainBlockDesctop;        
        &__block {
            position: relative;
            width: $widthMainBlockDesctop;
            margin: 0 auto;
        }
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
                position: relative;
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 20px;
            }
            &-image {
                display: flex;
                flex-direction: column;
                justify-content: center;             
            }
            &-img {
                border-radius: 20px;
            }
            &-buttons {
                position: absolute;
                width: 635px;
                display: flex;
                justify-content: space-between;
                flex-direction: row;
            }
            &-backward {
                position: relative;
                display: flex;
                align-content: center;
                justify-content: center;
                align-items: center;
                flex-direction: row;
            }
            &-forward {
                position: relative;
                display: flex;
                align-content: center;
                justify-content: center;
                align-items: center;
                flex-direction: row;
            }
            &-circle1 {
                position: absolute;
                width: 80px;
                height: 80px;
                background-color: rgb(250, 252, 254, 0.5);
                border-radius: 50%;
            }
            &-circle2 {
                position: absolute;
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                left: 16px;
                top: 16px;
                width: 48px;
                height: 48px;
                border-radius: 50%;
                box-shadow: 0px 8px 16px 0px rgba(255, 107, 0, 0.16);
                background-color: rgb(255, 255, 255, 1);
            }
            &-arrow {
                width: 24px;
                height: 24px;
            }
        }
    }
</style>
