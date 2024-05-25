<template>
  <div id="app">
    <header class="header center">
      <img src="./assets/images/Logo.svg" alt="company logo" class="header__logo">
      <div class="header__categories">
        <span class="header__categories-item">Наши услуги</span>
        <span class="header__categories-item">О компании</span>
        <span class="header__categories-item">Отзывы</span>
        <span class="header__categories-item">Выполненные заказы</span>
        <span class="header__categories-item">Контакты</span>
      </div>
      <div class="header__adress">
        <img class="header__adress-img" src="./assets/images/drop.svg" alt="geo spot">
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
      <img src="./assets/images/phone-call.svg" alt="phone call icon" class="header__phoneCall">
    </header>
    <section class="mainBanner center">
      <div id="circle1"></div>
      <div id="circle2"></div>
      <div id="circle3"></div>
      <div class="mainBanner__master">        
        <div class="mainBanner__master-circle"></div>
        <div class="mainBanner__master-circle1"></div>
        <div class="mainBanner__master-monitor">
          <img src="./assets/images/circle3.svg" alt="monitor">
        </div>
        <div class="mainBanner__master-phone">
          <img src="./assets/images/circle4.svg" alt="phone">
        </div>
        <div class="mainBanner__master-gear">
          <img src="./assets/images/circle1.svg" alt="gear" id="gear-img">
        </div>
        <div class="mainBanner__master-laptop">
          <img src="./assets/images/circle2.svg" alt="laptop">
        </div>
        <img src="./assets/images/master-vector.svg" alt="vector element" class="mainBanner__master-vector">
        <img src="./assets/images/master2.png" alt="master image" class="mainBanner__master-image">
      </div>
      <div class="mainBanner__title">
        <div class="mainBanner__name">Проблемы с Вашим устройством?</div>
        <div class="mainBanner__subtitle">Решаем любые проблемы!<br>Большой склад и опытные мастера</div>
        <div class="mainBanner__button">Бесплатная консультация</div>
      </div>
      <div class="mainBanner__elements">
        <img src="./assets/images/wave.svg" alt="waves" class="mainBanner__elements-waves">
        <img src="./assets/images/grey-arrows.svg" alt="arrow" class="mainBanner__elements-arrow">
        <img src="./assets/images/ellipse.svg" alt="ellipse" class="mainBanner__elements-ellipse">
        <img src="./assets/images/dots.svg" alt="dots" class="mainBanner__elements-dots">
      </div>
      <div class="mainBanner__action">
        <div class="mainBanner__discount">
          <span class="mainBanner__discount-text">50%</span>
          <img src="./assets/images/fire.svg" class="mainBanner__discount-image" alt="fire image">
        </div>
        <div class="mainBanner__content">
          скидка на ремонт телефонов, ноутбуков и планшетов до <b>-50%</b>
        </div>
        <hr class="mainBanner__line">
        <div class="mainBanner__counter">
          <p class="mainBanner__counter-title">Конец акции:</p>
          <div class="mainBanner__counter-content">
          <div class="mainBanner__counter-item">
            <span class="item-value">2</span><br>
            <span class="item-title">DAYS</span>
          </div>
          <div class="mainBanner__counter-devider">:</div>
          <div class="mainBanner__counter-item">
            <span class="item-value">18</span><br>
            <span class="item-title">HOURS</span>
          </div>
          <div class="mainBanner__counter-devider">:</div>
          <div class="mainBanner__counter-item">
            <span class="item-value">56</span><br>
            <span class="item-title">MINUTES</span>
          </div>
        </div>
        </div>
      </div>
      <div class="mainBanner__advantages">
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/truck.svg" alt="truck image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Курьер по городу</div>
          <div class="mainBanner__advantages-content">Выезд курьера Буюканы Чеканы, Рышкановка, центр, Ботаника.</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/replace-phone.svg" alt="replace-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Подменный телефон - Бесплатно</div>
          <div class="mainBanner__advantages-content">Телефон взамен Беслатно, пока ваш в ремонте</div>
        </div>
        <div class="mainBanner__advantages-item">
          <img src="./assets/images/adv-phone.svg" alt="adv-phone image" class="mainBanner__advantages-image">
          <div class="mainBanner__advantages-title">Забота о вас</div>
          <div class="mainBanner__advantages-content">Незначительные поломки - делаем бесплатно.</div>
        </div>
      </div>
    </section>

    <section class="service center">
      <div class="span-col">
        <div class="service-circle"></div>
        <div class="service__title">Мы работаем <br> с устройствами:</div>
      </div>
      <div class="service__item" id="apple">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/dots_45.svg" alt="dots" class="service__item-vector">
        <img src="./assets/images/apple.png" alt="apple image" class="service__item-img">
        <div class="service__item-logoCircle"></div>
        <img src="./assets/images/apple-logo.svg" alt="apple logo image" class="service__item-logo">      
        <div class="service__item-title">Apple</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="android">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/wave.svg" alt="waves" class="service__item-vector">
        <img src="./assets/images/android.png" alt="android image" class="service__item-img">
        <div class="service__item-logoCircle"></div>
        <img src="./assets/images/android-logo.svg" alt="android logo image" class="service__item-logo">      
        <div class="service__item-title">Android</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="gadgets">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/wave.svg" alt="waves" class="service__item-vector">
        <img src="./assets/images/gadgets.png" alt="gadgets image" class="service__item-img">
        <div class="service__item-title">Гаджетами</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="laptop">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/triangle.svg" alt="triangle" class="service__item-vector">
        <img src="./assets/images/laptop.png" alt="laptop image" class="service__item-img">
        <div class="service__item-title">Ноутбуками</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>

      <div class="service__item" id="pc">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/yellow-arrows.svg" alt="yellow-arrows" class="service__item-vector">
        <img src="./assets/images/pc.png" alt="pc image" class="service__item-img">
        <div class="service__item-title">Моноблоками и РС</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>
      
      <div class="service__item" id="devices">
        <div class="service__item-rectangle"></div>
        <img src="./assets/images/grey_triangle.svg" alt="grey_triangle" class="service__item-vector">
        <img src="./assets/images/devices.png" alt="devices image" class="service__item-img">
        <div class="service__item-title">Другими устройствами</div>
        <div class="arrow-circle2"></div>
        <div class="arrow-circle1"></div>
        <img src="./assets/images/chevron-right.svg" alt="arrow" class="service__item-arrow">
      </div>
    </section>

    <section class="aboutCompany center">
      <div class="aboutCompany__left">
        <img src="./assets/images/grey-arrows.svg" alt="grey arrows image" class="aboutCompany__vector">
        <div class="aboutCompany__title">О компании Arron</div>
        <div class="aboutCompany__subtitle">Узнайте больше о нашей компании из видео за 1 минуту.</div>
        <div class="aboutCompany__button">
          <p class="aboutCompany__button-name">Смотреть</p>
          <img src="./assets/images/play-white.svg" alt="play image" class="aboutCompany__button-img">
        </div>
      </div>
      <div class="aboutCompany__right">
        <div class="aboutCompany__right-card">
          <img src="./assets/images/truck.svg" alt="truck image">
          <p class="aboutCompany__right-cardTitle">Выезжаем в любую точку Кишинева</p>
          <p class="aboutCompany__right-cardText">Выезд курьера Буюканы, Чеканы,<br>Рышкановка, центр, Ботаника.</p>          
        </div>
        <div class="aboutCompany__right-card">
          <img src="./assets/images/clock.svg" alt="clock image">
          <p class="aboutCompany__right-cardTitle">Работы от 30 минут</p>
          <p class="aboutCompany__right-cardText">Время работы или настройки занимает<br>от 30 минут до нескольких часов.</p>    
        </div>
        <div class="aboutCompany__right-card">
          <img src="./assets/images/money.svg" alt="money image">
          <p class="aboutCompany__right-cardTitle">Удобный способ оплаты</p>
          <p class="aboutCompany__right-cardText">Оплата наличными или по<br>перечислению компаниям.</p>    
        </div>
        <div class="aboutCompany__right-card">
          <img src="./assets/images/shild.svg" alt="shild image">
          <p class="aboutCompany__right-cardTitle">Гарантия на все выполненные услуги</p>
          <p class="aboutCompany__right-cardText">Запчасти, фотографии и сообщения<br>под Вашим контролем. После работ<br>инженер отдаст Вам старые запчасти.</p>    
        </div>
      </div>
      <img src="./assets/images/wave.svg" alt="wave image" class="aboutCompany__wave">
    </section>


    <section class="feedback center">
      <img src="./assets/images/ellipse.svg" alt="ellipse image" class="feedback__vector1">
      <img src="./assets/images/dots.svg" alt="dots image" class="feedback__vector2">
      <div class="feedback__header">
        <div class="feedback__title">Отзывы счастливых клиентов</div>
        <div class="carousel__buttons">
          <div class="buttonCircle">
            <img src="./assets/images/chevron-left.svg" alt="left button arrow" class="buttonCircle-left">
          </div>
          <div class="buttonCircle">
            <img src="./assets/images/chevron-right.svg" alt="right bbuttonCircleutton arrow" class="buttonCircle-right">
          </div>
        </div>
      </div>

      <div class="feedback__content">
        <div class="feedback__content-item">
          <img src="./assets/images/feedback_1.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="./assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="./assets/images/feedback_2.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="./assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="./assets/images/feedback_3.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="./assets/images/play.svg" alt="play image" class="feedback__btn-play">
          </div>
        </div>
        <div class="feedback__content-item">
          <img src="./assets/images/feedback_4.jpg" alt="feedback snap image" class="feedback__img">
          <div class="feedback__btn">
            <div class="feedback__btn-circle1"></div>
            <div class="feedback__btn-circle2"></div>
            <img src="./assets/images/play.svg" alt="play image" class="feedback__btn-play">
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

    <section class="complOrders center"></section>

    <!-- <section class="arronService center">
      <div class="arronService__vector"></div>
      <img src="./assets/images/ellipse.svg" alt="check list icon" class="arronService__vector1">
      <img src="./assets/images/dots.svg" alt="check list icon" class="arronService__vector2">
      <div class="arronService__content">
        <div class="arronService__left">
          <p class="arronService__title">что делать если ноутбук или телефон медленно работает</p>
          <div class="arronService__solution">
            <img src="./assets/images/check_list_icon.svg" alt="check list icon" class="arronService__icon">
            <p class="arronService__text">Получите чек лист - Что делать, если ноутбук или телефон грузится</p>
          </div>          
          <div class="arronService__button">Получить чек лист</div>          
        </div>
        <div class="arronService__right">
          <div class="arronService__right-item">
            <p class="arronService__title">Наши услуги</p>
            <ul class="arronService__list">
              <li>ремонт ноутбуков</li>
              <li>ремонт смартфонов</li>
              <li>заправка и ремонт картриджей</li>
              <li>установка СНПЧ</li>
              <li>ремонт компьютеров</li>
              <li>ремонт моноблоков</li>
            </ul>
          </div>
          <div class="arronService__right-item">
            <ul class="arronService__list">
              <li>ремонт планшетов</li>
              <li>ремонт КПК</li>
              <li>ремонт принтеров</li>
              <li>ремонт роутеров</li>
              <li>всстановление жестких дисков</li>
              <li>компьютерная помощь и IT аутсорсинг и др.</li>
            </ul>
          </div>       
        </div>
      </div>
    </section> -->

    <section class="gifts center"></section>
    <section class="about center"></section>
    <section class="lid center"></section>

    <!-- <footer class="footer center">Lorem, ipsum dolor.</footer> -->
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {

  }
}
</script>

<style lang="scss">
#app {
  $widthSiteDesctop: 1920px;
  $commonBgColor: #f4f9fc;
  $mainTextColor: #13171D;
  $mainBannerSubtitleColor: #444444;
  $buttonTextColor: white;
  $buttonColor: #E2001A;
  $discountTextColor: #FF6b00;

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
  
  // a {
  //   text-decoration: none;
  // }

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

  .mainBanner {
    position: relative;
    margin-left: 74px;
    margin-right: 58px;
    height: 1118px;
    width: 1788px;
    &__title {
      width: 635px;     
      position: absolute;
      left: 277px;
      top: 295px;
    }
    &__name {
      @include textDecoration("Bebas Neue", 700, 100px, 100px, calc(1em * -0.08));
      color: $mainTextColor;
    }
    &__subtitle {
      padding-top: 20px;
      padding-bottom: 40px;
      @include textDecoration(Gilroy, 400, 24px, 34px, calc(1em * -0.01));
      color: $mainBannerSubtitleColor;
    }
    &__button {
      width: 224px;
      height: 28px;
      @include textDecoration(Montserrat, 600, 16px, 26px, calc(1em * -0.01));
      color: $buttonTextColor;
      background: rgb(226,0,26);
      border-radius: 15px;
      padding: 18px 30px;
      outline: none;
      user-select: none;
    }
    &__button:hover {
      color: $buttonColor;
      border: 2px solid $buttonColor;
      background: rgb(255,255,255);
    }
    &__master {
      position: absolute;
      left: -3px;
      top: -42px;
      &-vector {
        position: absolute;
        left: 1287.7px;
        top: 206.7px;
        border: 1px solid rgb(19, 23, 29);
        visibility: hidden;
      }
      &-image {
        position: absolute;
        left: 965px;
        top: 239px;
      }
      &-circle {
        position: absolute;
        border-radius: 247.55px;
        width: 495.09px;
        height: 495.09px;
        left: 974.16px;
        right: -704.24px;
        top: 406.48px;
        bottom: -50.29px;
        background: linear-gradient(180.00deg, rgb(0, 90, 170),rgb(61, 138, 255) 100%);
      }
      &-circle1 {
        position: absolute;
        width: 765px;
        height: 765px;
        border-radius: 382.5px;
        left: 839.16px;
        top: 271.56px;
        border: 2px dashed rgb(0, 0, 0);
        opacity: 0.3;
      }
      &-monitor {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 29.27px;
        width: 58.54px;
        height: 58.54px;
        left: 1434.66px;
        right: -1434.66px;
        top: 915.29px;
        bottom: -915.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
      }
      &-phone {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 36.27px;
        width: 72.54px;
        height: 72.54px;
        left: 840.89px;
        right: -840.89px;
        top: 778.29px;
        bottom: -778.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
      }
      &-gear {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 42.27px;
        width: 84.54px;
        height: 84.54px;
        left: 966.89px;
        right: -966.89px;
        top: 292.29px;
        bottom: -292.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);
       
      }
      &-laptop {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        border-radius: 25.27px;
        width: 50.54px;
        height: 50.54px;
        left: 1425.66px;
        right: -1425.66px;
        top: 318.29px;
        bottom: -318.29px;
        box-shadow: 0px 10px 10px 0px rgba(255, 107, 0, 0.05),0px 20px 40px 0px rgba(255, 107, 0, 0.13);
        background: rgb(255, 255, 255);        
      }
    }
    &__elements {
      position: relative;
      width: 1788px;
      height: 585.5px;
      top: 363.6px;
      &-waves {
        position: absolute;
        left: 1586.5px;
        top: 0px;
      }
      &-arrow {
        position: absolute;
        left: 701.5px;
        top: 47.6px;
      }
      &-dots {
        position: absolute;
        right: -54.6px;
        top: 506.5px;
      }
      &-ellipse {
        position: absolute;
        left: 0px;
        top: 535.5px;
      }
    }
    &__action {
      position: absolute;
      left: 1340.16px;
      right: 183.62px;
      top: 431.29px;
      bottom: 339.83px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      width: 204px;
      height: 309px;
      background-color: white;
      border-radius: 30px;
      padding-left: 30px;
      padding-right: 30px;
    }
    &__discount {
      margin-top: -38px;
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      gap: 21px;
      &-text {
        @include textDecoration('Bebas Neue', 700, 113px, 113px, calc(1em * -0.01));
        color: $discountTextColor;
      }
      &-image {
        width: 24px;
        height: 32px;
        margin-bottom: 20px;
      }
    }
    &__content {
      @include textDecoration(Gilroy, 400, 18px, 26px);
       color: $mainTextColor;
    }
    &__line {
      margin-top: 22px;
      margin-bottom: 22px;
      color: rgba(19, 23, 29, 0.5);
      width: 204px;
    }
    &__counter {
      &-title {
        margin: 0px;
        @include textDecoration(Gilroy, 600, 20px, 24px, calc(1em * -0.01));
        color: rgba(19, 23, 29, 0.5);
      }
      &-content {
        display: flex;
        flex-direction: row;
        gap: 6px;
      }
      &-item {
        width: 48px;
      }
      &-devider {
        @include textDecoration(Gilroy, 600, 32px, 38px, calc(1em * -0.01));
        color: $mainTextColor;
      }
    }
    &__advantages {
      position: relative;
      width: 1298px;
      height: 192px;
      left: 311px;
      top: 400px;
      display: flex;
      justify-content: space-between;
      &-item {
        width: 364px;
        display: flex;
        flex-direction: column;
      }
      &-image {
        width: 80px;
        height: 80px;
      }
      &-title {
        @include textDecoration(Gilroy, 600, 20px, 24px);
        color: $mainTextColor;
        margin-top: 24px;
        margin-bottom: 16px;
      }
      &-content {
        @include textDecoration(Gilroy, 400, 18px, 24px);
        color: $mainBannerSubtitleColor;        
      }
    }

  }
  .item-value {
    text-align: center;
    @include textDecoration(Gilroy, 600, 32px, 38px, calc(1em * -0.01));
        color: $mainTextColor;
  }
  .item-title {
    @include textDecoration(Gilroy, 600, 11px, 13px, calc(1em * -0.01));
    color: rgba(19, 23, 29, 0.5);
  }

  #gear-img {
    opacity: 0.1;
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
      @include textDecoration("Bebas Neue", 700, 80px, 84px, calc(1em * -0.25));
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
        // width: 77.7px;
        // height: 77.7px;
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

  .aboutCompany {
    position: relative;
    display: flex;
    flex-direction: row;
    gap: 110px;
    height: 545px;
    // width: 1298px;
    margin: 0 auto;
    background: linear-gradient(180.00deg, rgb(235, 243, 248),rgba(235, 243, 248, 0) 100%);
    &__left {
      position: relative;
      padding-left: 311px;
      padding-top: 80px;
      width: 333px;
      height: 402px;
      display: flex;
      flex-direction: column;
    }
    &__title {
      text-transform: uppercase;
      @include textDecoration("Babes Neue", 700, 80px, 80px, calc(1em * -0.35));
      color: $mainTextColor;
    }
    &__subtitle {
      padding-top: 24px;
      padding-bottom: 64px;
      @include textDecoration(Gilroy, 400, 24px, 30px);
      color: $mainBannerSubtitleColor;
    }
    &__vector {
      position: absolute;
      left: 537px;
      top: 186px;
    }
    &__button {
      display: flex;
      flex-direction: row;
      align-items: center;
      gap: 16px;
      padding: 18px 30px;
      width: 122px;
      height: 28px;
      border-radius: 15px;
      background: rgb(226, 0, 26);
      &-name {
        @include textDecoration(Montserrat, 600, 16px, 26px);
        color: $buttonTextColor;
      }
      &-img {
        width: 14px;
        height: 18px;
      }
    }
    &__right {
      padding-top: 97px;
      width: 788px;
      margin-right: 75px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: 1fr 1fr;
      row-gap: 40px;
      column-gap: 80px;
      &-card {
        display: inline-block;
      }
      &-cardTitle {
        @include textDecoration(Gilroy, 600, 20px, 24px);
        color: $mainTextColor;
      }
      &-cardText {
        @include textDecoration(Gilroy, 400, 18px, 24px);
        color: $mainBannerSubtitleColor;
      }
    }
    &__wave {
      position: absolute;
      left: 1645px;
      top: 417px;
      width: 98px;
    }
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
    width: 1300px;
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
  
  .arronService {
    position: relative;
    margin: 0 auto;
    width: 1476px;
    margin-top: -65px;
    padding-top: 160px;
    &__content {
      padding-left: 126px;
      padding-right: 134px;
      display: flex;
      flex-direction: row;
      gap: 125px;
      align-items: center;
    }
    &__left {
      max-width: 427px;
      display: flex;
      flex-direction: column;
    }
    &__title {
      text-transform: uppercase;
      margin: 0 0;
      @include textDecoration("Babes Neue", 700, 48px, 48x, calc(1em * -0.3));
      color: $mainTextColor;
    }
    &__icon {
      width: 35px;
      height: 45px;
    }
    &__text {
      @include textDecoration(Montserrat, 400, 14px, 17x);
      color: black;
    }
    &__solution {
      width: 333px;
      padding-top: 6px;
      padding-bottom: 32px;
      display: flex;
      flex-direction: row;
      align-items: center;
      gap: 10px;
    }
    &__button {
      text-align: center;
      padding: 29px 35px 24px;
      width: 260px;
      height: 28px;
      border-radius: 15px;
      background: $buttonColor;
      @include textDecoration(Montserrat, 600, 16px, 26px);
      color: $buttonTextColor;
    }
    &__right {
      display: flex;
      flex-direction: row;
      gap: 32px;
      align-items: center;
      &-item{
        display: inline-block;
      }
    }
    &__list li {
      padding-bottom: 18px;
      @include textDecoration(Montserrat, 400, 18px, 24px);
      color: $mainBannerSubtitleColor;
    }
    &__list li::marker {
      color: $buttonColor;
      font-size: 24px;
    }
    &__vector {
      position: absolute;
      width: 276px;
      height: 276px;
      left: 0px;
      top: 0px;      
      background: conic-gradient(from 180deg at 50% 50%, rgb(238, 243, 248), rgba(238, 243, 248, 0));
      border-radius: 50%;
    }
    &__vector2 {
      position: absolute;
      left: 1294px;
      top: 69px;
    }
    &__vector1 {
      position: absolute;
      left: 1426px;
      top: 490px;
    }
  }



}
</style>
