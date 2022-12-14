<template>
  <div class="wrapper">
    <HeaderMain />
    <ServicesPage />
    <AdvantagesPage />
    <PracticePage />
    <WhowearePage />
    <ClientsPage />
    <SubscribePage />
    <GetintouchPage />
    <ContactPage />
    <FooterPage />
  </div>
</template>

<script>
import HeaderMain from "./components/HeaderMain.vue";
import ServicesPage from "./components/ServicesPage.vue";
import AdvantagesPage from "./components/AdvantagesPage.vue";
import PracticePage from "./components/PracticePage.vue";
import WhowearePage from "./components/WhowearePage.vue";
import ClientsPage from "./components/ClientsPage.vue";
import SubscribePage from "./components/SubscribePage.vue";
import GetintouchPage from "./components/GetintouchPage.vue";
import ContactPage from "./components/ContactPage.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
  name: "App",
  components: {
    HeaderMain,
    ServicesPage,
    AdvantagesPage,
    PracticePage,
    WhowearePage,
    ClientsPage,
    SubscribePage,
    GetintouchPage,
    ContactPage,
    FooterPage,
  },
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
._ibg {
  position: relative;
}
._ibg img {
  position: absolute;
  top: 0;
  left: 0;
  object-fit: cover;
}
</style>
