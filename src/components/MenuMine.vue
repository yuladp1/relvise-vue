<template>
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
</template>

<script>
export default {
  name: "MenuMine",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style>
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
</style>
