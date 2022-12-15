<template>
  <div class="wrapper__header-and-main">
    <div class="wrapper__header _container">
      <header class="header__container" v-bind:class="{ 'icon-mobile-view': mobileNav }">
        <a class="header__logo">Relvise</a>
        <nav class="header__menu menu">
          <ul class="menu__list" v-show="!mobile">
            <li class="menu__item"><a href="" class="menu__link">Home</a></li>
            <li class="menu__item"><a href="" class="menu__link">Product</a></li>
            <li class="menu__item"><a href="" class="menu__link">Pricing</a></li>
            <li class="menu__item"><a href="" class="menu__link">Contact</a></li>
          </ul>

          <transition name="mobile-nav">
            <ul class="dropdown-nav" v-show="mobileNav">
              <li class="link">Home</li>
              <li class="link">Product</li>
              <li class="link">Pricing</li>
              <li class="link">Contact</li>
            </ul>
          </transition>
        </nav>
        <div class="icon" v-on:click="toggleMobileNav" v-show="mobile"></div>
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
            <a href="" class="main-block__button main-block__button-border">Learn more</a>
          </div>
        </div>
      </div>
    </main>
    <div class="main-block__image _ibg">
      <img src="../assets/images/main-block/cover-main-block.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderMain",
  data() {
    return {
      scrollPosition: null,
      mobile: false,
      mobileNav: null,
      windowWidth: null,
    };
  },
  created() {
    window.addEventListener("resize", this.checkScreen);
  },
  methods: {
    toggleMobileNav() {
      this.mobileNav = !this.mobileNav;
    },
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 992) {
        this.mobile = true;
        return;
      } else {
        this.mobile = false;
        this.mobileNav = false;
        return;
      }
    },
  },
};
</script>

<style scoped>
.icon {
  background-image: url("../assets/images/hamburger-menu.png");
  /* display: flex; align-items: center;*/
  width: 30px;
  height: 30px;
  background-size: cover;
}
.icon-mobile-view {
  display: flex;
  justify-content: space-between;
}
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
@media (max-width: 992px) {
  .header__container {
    display: flex;
    justify-content: space-between;
  }
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
@media (max-width: 992px) {
  header__container {
    display: flex;
    justify-content: space-between;
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
.dropdown-nav {
  margin: 0;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  align-content: space-around;
  position: absolute;
  width: 120px;
  background-color: white;
  top: 104px;
  right: 0;
  padding: 30px 0 30 20px;
}
.dropdown-nav li {
  color: black;
  padding: 10px;
}

.mobile-nav-enter-active,
.mobile-nav-leave-active {
  transition: 1s ease all;
}
.mobile-nav-enter-from,
.mobile-nav-enter-to {
  transform: translate(250px);
}
.mobile-nav-enter-to {
  transform: translate(0);
}
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
.main-block__button-orange:hover {
  background-color: white;
  color: #ff7b47;
  border: 1px solid #ff7b47;
  transition: all 0.3s ease 0.2s;
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
.main-block__button-border:hover {
  background: #0d5c63;
  color: white;
  transition: all 0.3s ease 0.2s;
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
</style>
