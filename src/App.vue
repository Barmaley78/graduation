<template>
  <div id="app">
    <headerComponent />
    <mainBannerComponent />
    <serviceComponent />
    <abounCompanyComponent />
    <feedbackComponent />
    <complOrdersComponent />
    <arronServiceComponent />
    <giftsComponent />
    <aboutComponent />
    <lidComponent />
    <footerComponent />
  </div>
</template>

<script>

import headerComponent from './components/headerComponent.vue'
import mainBannerComponent from './components/mainBannerComponent.vue'
import serviceComponent from './components/serviceComponent.vue'
import abounCompanyComponent from './components/abounCompanyComponent.vue'
import feedbackComponent from './components/feedbackComponent.vue'
import complOrdersComponent from './components/complOrdersComponent.vue'
import arronServiceComponent from './components/arronServiceComponent.vue'
import giftsComponent from './components/giftsComponent.vue'
import aboutComponent from './components/aboutComponent.vue'
import lidComponent from './components/lidComponent.vue'
import footerComponent from './components/footerComponent.vue'

  export default {
    name: 'App',
    components: {
      headerComponent,
      mainBannerComponent,
      serviceComponent,
      abounCompanyComponent,
      feedbackComponent,
      complOrdersComponent,
      arronServiceComponent,
      giftsComponent,
      aboutComponent,
      lidComponent,
      footerComponent
    }
  }
</script>

<style lang="scss">
#app {
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
}
</style>
