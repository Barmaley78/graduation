<template>
    <section class="lid center">
        <div class="lid__block">
            <div class="lid__content">
          <div class="lid__left">
            <div class="lid__discount">
              <div class="lid__discount-rect">&nbsp;</div>
              <span class="lid__discount-text">50%</span>

              <img src="../assets/images/fire.svg" class="lid__discount-image" alt="fire image">
            </div>
            <p class="lid__left-title">Записаться на<br>диагностику<br>в <span class="lid__left-title" id="colored">удобное</span> вам время</p>
          </div>

          <div class="lid__right">
            <input type="text" placeholder="День" class="lid__right-input">
            <input type="text" placeholder="Время" class="lid__right-input">
            <input type="text" placeholder="Телефон" class="lid__right-input span-col">
            <div class="lid__right-button">Записаться</div>
          </div>
      </div>
        </div>

    </section>
</template>

<script>
export default {
  name: 'lidComponent'
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

    .lid {
        margin: 0 auto;
        width: $widthMainBlockDesctop;
        margin-top: 58px;
        margin-bottom: 117px;        
        &__block {
            margin: 0 auto;
            width: $widthMainBlockDesctop;
            height: 326px;
            box-sizing: border-box;
            border: 1px solid rgb(199, 209, 215);
            border-radius: 30px;
        }
        &__content {
            width: 1078px;
            margin: 0 auto;
            display: flex;
            flex-direction: row;
            justify-content: space-between;
        }
        &__left {
            width: 397px;
            display: flex;
            flex-direction: column;
            &-title {
                text-transform: uppercase;
                @include textDecoration('Bebas Neue', 700, 48px, 48px);
                color: $mainTextColor;
            }
            &-title#colored {
                color: $buttonColor;
            }
            }
            &__discount {
                position: relative;
                margin-top: -58px;
                width: 190px;
                display: flex;
                flex-direction: row;
                align-items: flex-end;
                gap: 21px;
            &-text {
                z-index: 10;
                @include textDecoration('Bebas Neue', 700, 113px, 113px, calc(1em * -0.01));
                color: $discountTextColor;
                text-align: center;
            }
            &-rect {
                position: absolute;
                top: 42px;
                left: 0px;
                width: 197px;
                height: 32px;
                background: $commonBgColor;
            }
            &-image {
                width: 24px;
                height: 32px;
                margin-bottom: 90px;
            }
        }
        &__right {
            padding-top: 48px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr 1fr;
            row-gap: 20px;
            column-gap: 24px;
            &-input {
                height: 26px;
                border-radius: 15px;
                @include textDecoration(Montserrat, 400, 14px, 26px);
                border: 1px solid rgb(199, 209, 215);
                padding: 19px 24px 19px 24px;
            }
            &-button {
                width: 240px;
                height: 28px;
                border-radius: 15px;
                background: $buttonColor;
                text-align: center;
                @include textDecoration(Montserrat, 600, 16px, 28px);
                color: $buttonTextColor;
                padding: 18px 30px 18px 30px;
            }
        }
    }

    .span-col {
        position: relative;
        grid-column: auto / span 2;
    }
</style>
