<template>
    <header class="header center">
        <img src="../assets/images/Logo.svg" alt="company logo" class="header__logo">
        <div class="header__categories">
            <span class="header__categories-item">Наши услуги</span>
            <span class="header__categories-item">О компании</span>
            <span class="header__categories-item">Отзывы</span>
            <span class="header__categories-item">Выполненные заказы</span>
            <span class="header__categories-item">Контакты</span>
        </div>
        <div class="header__adress">
            <img class="header__adress-img" src="../assets/images/drop.svg" alt="geo spot">
            <div class="header__adress-content">
            <div class="header__adress-item">г. Кишинев, ул. Бэнулеску Бодони, д. 33</div>
            <div class="header__adress-link">Мы на карте</div>
            </div>
        </div>
        <div class="header__phoneNumber">
            <span class="header__phoneNumber-item">069 82 77 38</span>
            <span class="header__phoneNumber-item">/</span>
            <span class="header__phoneNumber-item">079 92 77 38</span>
        </div>
        <img src="../assets/images/phone-call.svg" alt="phone call icon" class="header__phoneCall">
    </header>
</template>
  
<script>
export default {
    name: 'headerComponent'
}
</script>

<style lang="scss" scoped>
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

    .header {
        margin-top: 30px;
        margin-left: 30px;
        margin-right: 30px;
        width: 1860px;
        display: flex;
        align-items: center;
        &__categories {
        @include textDecoration(Gilroy, 600, 16px, 19px, calc(1em * -0.01));
        color: $mainTextColor;
        padding-left: 78px;
        padding-right: 291px;
        display: flex;
        flex-direction: row;
        gap: 24px;
        }
        &__adress {      
        width: 330px;
        display: flex;
        flex-direction: row;
        gap: 16px;
        &-item{
            @include textDecoration(Montserrat, 400, 14px, 17px, calc(1em * -0.01));
        }
        &-link {
            @include textDecoration(Montserrat, 400, 12px, 15px, calc(1em * -0.01));
            color: blue;
            text-decoration: underline;
        }
        &-content {
            display: flex;
            flex-direction: column;
        }
        }
        &__phoneNumber {    
        width: 262px;
        padding-left: 45px;
        padding-right: 35px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        &-item {
            @include textDecoration(Gilroy, 600, 20px, 24px, calc(1em * -0.01));
        }
        }
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