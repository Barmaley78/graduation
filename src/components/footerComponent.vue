<template>
    <footer class="footer center">
        <p class="footer__title">Наши контакты</p>
        <div class="footer__media">
            <div class="footer__media-right">
                <div class="footer__media-image">
                    <img src="../assets/images/contacts1.jpg" alt="contacns image" class="footer__media-img">
                    <div class="footer__media-buttons">
                        <div class="footer__media-backward">
                            <div class="footer__media-circle1">
                                <div class="footer__media-circle2">
                                    <img src="../assets/images/chevron-left.svg" alt="" class="footer-arrow">
                                </div>              
                            </div>              
                        </div>
                        <div class="footer__media-forward">
                            <div class="footer__media-circle1">
                                <div class="footer__media-circle2">
                                    <img src="../assets/images/chevron-right.svg" alt="" class="footer-arrow">
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
            <div class="footer__media-video">
                <img src="../assets/images/contacts2.jpg" alt="contacns image" class="footer__img">
                <div class="footer__btn">
                    <div class="footer__btn-circle1">
                        <div class="footer__btn-circle2">
                            <img src="../assets/images/play.svg" alt="play image" class="footer__btn-play">
                        </div>            
                    </div>            
                </div>
            </div>
        </div>
        <div class="footer__contacts">
        <div class="footer__conts">
            <div class="footer__conts-item">
            <img src="../assets/images/phone-icon.svg" alt="" class="footer__conts-img">
            <p class="footer__conts-text">069 82 77 38 / 079 92 77 38</p>
            </div>
            <div class="footer__conts-item">
            <img src="../assets/images/email-icon.svg" alt="" class="footer__conts-img">
            <p class="footer__conts-text">info@arron.md</p>
            </div>
            <div class="footer__conts-item">
            <img src="../assets/images/drop-icon.svg" alt="" class="footer__conts-img">
            <p class="footer__conts-text">г. Кишинев, ул. Бэнулеску Бодони, д.33</p>
            </div>
        </div>

        <div class="footer__socials">
        <div class="footer__socials-rating">
            <p class="footer__socials-text">Рейтинг сервиса</p>
            <img src="../assets/images/stars.svg" alt="" class="footer__socials-img">
            <p>4.8/5.0 - 403 голоса</p>
        </div>
        <div class="footer__socials-nets">
            <p class="footer__socials-text">Мы в соцсетях</p>
            <div class="footer__socials-netsIcons">
            <img src="../assets/images/instagram.svg" alt="" class="footer__socials-icon">
            <img src="../assets/images/facebook.svg" alt="" class="footer__socials-icon">
            <img src="../assets/images/tiktok.svg" alt="" class="footer__socials-icon">
            <img src="../assets/images/youtube.svg" alt="" class="footer__socials-icon">

            </div>
        </div>
        </div>
        </div>
        <div class="footer__bgImage"></div>        
    </footer>
</template>

<script>
export default {
  name: 'footerComponent'
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

    .footer {
        margin: 0 auto;
        width: $widthMainBlockDesctop;
        &__title {
            text-transform: uppercase;
            @include textDecoration('Bebas Neue', 700, 56px, 56px);
            color: $mainTextColor;
            padding-bottom: 40px;
        }
        &__media {
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: flex-start;
            padding-bottom: 58px;
            &-right {
                position: relative;
                display: flex;
                flex-direction: column;
                align-items: center;
            }
            &-image {
                display: flex;
                flex-direction: column;
                justify-content: center;  
            }
            &-img {
            border-radius: 20px;
            padding-bottom: 17px;
            }
            &-buttons {
                position: absolute;
                width: 594px;
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

            &-video {
                position: relative;
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
            }        
        }
        &__img {
            border-radius: 20px;
        }
        &__btn {
            position: absolute;
            left: 261px;
            top: 252px;
            &-circle1 {
                position: relative;
                width: 72px;
                height: 72px;
                box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
                background-color: rgb(255, 255, 255, 0.5);
                border-radius: 50%;
            }
            &-circle2 {
              position: absolute;
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                left: 8px;
                top: 8px;
                width: 56px;
                height: 56px;
                box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
                background-color: rgb(255, 255, 255, 1);
                border-radius: 50%;
            }
            &-play {
                width: 10.5px;
                height: 13.5px;
            }
        }
        &__contacts {
            z-index: 15;
            width: $widthMainBlockDesctop;
            height: 290px;
            border-radius: 30px;
            box-shadow: 0px 8px 10px 0px rgba(255, 107, 0, 0.08),0px 50px 60px 0px rgba(255, 107, 0, 0.08);
            background: rgb(255, 255, 255);      
        }
        &__conts {
            width: 1160px;
            margin: 0 auto;
            padding-top: 55px;
            display: flex;
            flex-direction: row;
            gap: 50px;
            &-item {
                display: flex;
                flex-direction: row;
                gap: 16px;
            }
            &-img {
                width: 56px;
                height: 56px;
            }
            &-text {
                @include textDecoration(Montserrat, 500, 20px, 20px);
                color: $mainTextColor;
            }
        }
        &__socials {
            padding-top: 34px;
            padding-left: 71px;
            display: flex;
            flex-direction: row;
            gap: 188px;
            &-text {
                @include textDecoration(Montserrat, 600, 20px, 1px);
                color: $mainTextColor;
            }
            &-img {
                width: 190px;
                height: 30px;
            }
            &-text2 {
                @include textDecoration(Gilroy, 400, 18px, 24px);
                color: $mainBannerSubtitleColor;
            }
            &-icon {
                width: 35px;
                height: 35px;
            }
            &-rating {
                width: 215px;
            }
            &-nets {
                width: 185px;
            }
            &-netsIcons {
                padding-top: 5px;
                display: flex;
                flex-direction: row;
                gap: 15px;
            }
        }
        &__bgImage {
            width: $widthSiteDesctop;
            height: 750px;
            z-index: -10;
            position: relative;
            margin-top: -80px;
            margin-left: -310px;
            background-image: url("../assets/images/map.jpg");
        }
    }
</style>
