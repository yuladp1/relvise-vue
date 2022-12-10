<template>
  <div class="wrapper">
    <div class="wrapper__header-and-main">
      <div class="wrapper__header _container">
        <header class="header__container">
          <a class="header__logo">Relvise</a>
          <nav class="header__menu menu">
            <ul class="menu__list">
              <li class="menu__item"><a href="" class="menu__link">Home</a></li>
              <li class="menu__item"><a href="" class="menu__link">Product</a></li>
              <li class="menu__item"><a href="" class="menu__link">Pricing</a></li>
              <li class="menu__item"><a href="" class="menu__link">Contact</a></li>
            </ul>
          </nav>
        </header>
      </div>
      <main class="page">
        <div class="page__wrapper _container">
          <div class="page__main-block main-block">
            <h1 class="main-block__title">Finance and Consultancy Solution</h1>
            <article class="main-block__text">
              We know how large objects will act, but things on a small scale.
            </article>
            <div class="main-block__buttons">
              <a href="" class="main-block__button main-block__button-orange"
                >Get Quote Now</a
              >
              <a href="" class="main-block__button main-block__button-border"
                >Learn more</a
              >
            </div>
          </div>
        </div>
      </main>
      <div class="main-block__image _ibg">
        <img src="./assets/images/main-block/cover-main-block.jpg" alt="" />
      </div>
    </div>

    <section class="page__services services">
      <div class="services__container _container">
        <div class="services__body">
          <div class="services__column">
            <div class="services__item item-services">
              <div class="item-services__icon">
                <img src="./assets/images/services/1.svg" alt="" />
              </div>
              <h2 class="item-services__title">Environmental Consulting</h2>
              <h3 class="item-services__text">
                We focus on ergonomics and meeting you where you work.
              </h3>
            </div>
            <div class="services__item item-services">
              <div class="item-services__icon">
                <img src="./assets/images/services/2.svg" alt="" />
              </div>
              <h2 class="item-services__title">Finance and consultancy</h2>
              <h3 class="item-services__text">
                Just type what's on your mind and we'll get you there.
              </h3>
            </div>
            <div class="services__item item-services item-services-green">
              <div class="item-services__icon">
                <img src="./assets/images/services/3.svg" alt="" />
              </div>
              <h2 class="item-services__title">Financial Services Consulting</h2>
              <h3 class="item-services__text">the quick fox jumps over the lazy dog</h3>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="page__advantages advantages">
      <div class="advantages__container _container">
        <div class="advantages__header header-block">
          <h2 class="header__block-title">Designing Better Experience</h2>
          <h3 class="header__block-text">
            Problems trying to resolve the conflict between the two major realms <br />
            of Classical physics: Newtonian mechanics
          </h3>
        </div>
        <div class="advantages__body">
          <div class="advantages__column">
            <div class="advantages__item">
              <div class="advantages__icon">
                <img src="./assets/images/advertise/1.svg" alt="" />
              </div>
              <div class="advantages__value">972 +</div>
              <div class="advantages__text">Consumer Products</div>
            </div>
          </div>

          <div class="advantages__column">
            <div class="advantages__item">
              <div class="advantages__icon">
                <img src="./assets/images/advertise/2.svg" alt="" />
              </div>
              <div class="advantages__value">181 +</div>
              <div class="advantages__text">Financial Services</div>
            </div>
          </div>
          <div class="advantages__column">
            <div class="advantages__item">
              <div class="advantages__icon">
                <img src="./assets/images/advertise/3.svg" alt="" />
              </div>
              <div class="advantages__value">98 %</div>
              <div class="advantages__text">Environmental</div>
            </div>
          </div>
          <div class="advantages__column">
            <div class="advantages__item">
              <div class="advantages__icon">
                <img src="./assets/images/advertise/4.svg" alt="" />
              </div>
              <div class="advantages__value">746 +</div>
              <div class="advantages__text">Business & Finance</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="page__practice practice">
      <div class="practice__container _container">
        <div class="practice__header header-block">
          <h2 class="header__block-title">Practice Advice</h2>
          <h3 class="header__block-text">
            Problems trying to resolve the conflict between <br />
            the two major realms of Classical physics: Newtonian mechanics
          </h3>
        </div>
      </div>
    </section>
    <footer class="footer">footer</footer>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Montserrat:100,200,300,regular,500,600,700,800,900,100italic,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic&display=swap);
@import url("./normalize.css");
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.wrapper {
  font-family: "Montserrat";
  min-height: 100%;
  overflow: hidden;
  color: #252b42;
  position: relative;
  display: flex;
  flex-direction: column;
  letter-spacing: 0.2px;
  background-color: #fafafa;
}
wrapper__header-and-main {
  position: absolute;
}
._container {
  max-width: 1016px;
  margin: 0 auto;
  padding: 0 15px 0 15px;
}
/* HEADER STYLES */
.wrapper__header {
  position: relative;
  width: 100%;
  min-height: 104px;
  max-height: 104px;
}
.header__container {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  display: flex;
  align-items: center;
  z-index: 10;
  width: 100%;
  padding: 0 15px;
}

.header__logo {
  font-family: Montserrat;
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
  letter-spacing: 0.1px;
}
.header__menu {
  margin: 0 0 0 134px;
  padding: 5px 0;
}
@media (max-width: 992px) {
  .header__menu {
    margin: 0 0 0 80px;
  }
}
@media (max-width: 767px) {
  .header__menu {
    margin: 0 0 0 40px;
  }
}
.menu__list {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
.menu__item:not(:last-child) {
  margin: 0 31px 0 0;
}
.menu__link {
  line-height: 24px;
  font-weight: 600;
  color: #737373;
}
/* HEADER STYLES -end */

/* MAIN STYLES */
page {
  flex: 1 1 auto;
  position: relative;
}
.page__wrapper {
  padding: 80px 15px 191px 15px;
  z-index: 50;
  position: relative;
}
@media (max-width: 992px) {
  .page__wrapper {
    padding: 30px 15px 191px 15px;
  }
}
.page__main-block {
  max-width: 509px;
  display: flex;
  flex-direction: column;
  align-content: flex-start;
  position: relative;
}

.page__main-block > *:not(:last-child) {
  margin: 0 0 35px 0;
}
.main-block__title {
  font-size: 58px;
  font-weight: 800;
  line-height: 80px;
  text-align: left;
}
@media (max-width: 992px) {
  .main-block__title {
    padding: 30px 15px 40px 15px;
    font-size: 48px;
  }
}
.main-block__text {
  font-size: 20px;
  font-weight: 500;
  line-height: 30px;
  text-align: left;
  max-width: 400px;
}
@media (max-width: 992px) {
  .main-block__text {
    color: #252b42;
    font-size: 28px;
  }
}
.main-block__buttons {
  display: inline-flex;
}
@media (max-width: 992px) {
  .main-block__buttons {
    flex-wrap: wrap;
  }
}

.main-block__button {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 36px;
  font-size: 14px;
  font-weight: 700;
  border-radius: 37px;
  flex: 0 1 50%;
}
@media (max-width: 992px) {
  .main-block__button {
    flex: 1 1 100%;
    min-height: 50px;
  }
}
.main-block__button:not(:last-child) {
  margin: 0 10px 0 0;
}
@media (max-width: 992px) {
  .main-block__button:not(:last-child) {
    margin: 20px 0;
  }
}
.main-block__button-orange {
  background-color: #ff7b47;
  color: white;
}
@media (max-width: 992px) {
  .main-block__button-orange {
    margin-bottom: 10px;
  }
}
.main-block__button-border {
  border: 1px solid #0d5c63;
  color: #0d5c63;
}
._ibg {
  position: relative;
}
._ibg img {
  /*position: absolute; */
  top: 0;
  left: 0;
  object-fit: cover;
}
.main-block__image {
  position: absolute;
  width: 100%;
  height: 100;
  top: 0;
  left: 0;
  object-fit: cover;
}
@media (max-width: 1300px) {
  .main-block__image img {
    object-fit: right;
  }
}
@media (max-width: 992px) {
  .main-block__image img {
    opacity: 0.2;
  }
}
/* SERVICES */
.page__services {
  z-index: 5;
}
.services__body {
  display: flex;
  margin: 0 -15px;
  z-index: 5;
}
.services__container {
  margin-top: -110px;
  z-index: 5;
}
.services__column {
  padding: 0 15px;
  display: flex;
  flex-wrap: wrap;
  height: 100%;
}

.services__item {
  padding: 35px 40px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  text-align: left;
  flex: 0 1 33.333%;
  background-color: white;
  height: 100%;
}

@media (max-width: 992px) {
  .services__item {
    flex: 0 1 50%;
    margin: 0 0 30px 0;
  }
}
@media (max-width: 670px) {
  .services__item {
    flex: 0 1 100%;
    margin: 0 15px 15px 15px;
  }
}
.item-services-green {
  background-color: #0d5c63;
}
.item-services-green > .item-services__title {
  color: white;
}
.item-services-green > .item-services__text {
  color: white;
}
.item-services > *:not(:last-child) {
  padding: 10px 0;
}

.item-services__title {
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  letter-spacing: 0.1px;
  color: #252b42;
}
.item-services__text {
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  letter-spacing: 0.2px;
  color: #737373;
}
/* ADVANTAGES */
.advantages {
  padding: 80px 0 0 0;
}
.advantages__header {
  margin: 0 0 50px 0;
}

.header__block-title {
  font-weight: 700;
  font-size: 40px;
  line-height: 57px;
}
.header__block-title:not(:last-child) {
  margin: 0 0 10px 0;
}
.header__block-text {
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  color: #737373;
}
.advantages__body {
  margin: 0 -15px;
  display: flex;
  flex-wrap: wrap;
}
.advantages__column {
  padding: 0 15px;
  display: flex;
  flex: 0 1 25%;
  display: flex;
  justify-content: center;
}
@media (max-width: 1000px) {
  .advantages__column {
    flex: 1 0 50%;
  }
}
@media (max-width: 560px) {
  .advantages__column {
    flex: 1 0 100%;
  }
}
.advantages__item {
  background-color: white;
  margin: 0 0 10px 0;
  flex-basis: 240px;
}
.advantages__item > *:not(:last-child) {
  padding: 0 0 10px 0;
}
.advantages__icon {
  height: 52px;
  display: flex;
  align-items: flex-end;
  justify-content: center;
}
.advantages__value {
  font-weight: 700;
  font-size: 40px;
  line-height: 57px;
}
.advantages__text {
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.1px;
  color: #737373;
}

/* FOOTER */
</style>
