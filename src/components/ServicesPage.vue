<template>
  <section class="page__services services">
    <div class="services__container _container">
      <div class="services__body">
        <div class="services__column">
          <div class="services__item item-services">
            <div class="item-services__icon">
              <img src="../assets/images/services/1.svg" alt="" />
            </div>
            <h2 class="item-services__title">Environmental Consulting</h2>
            <h3 class="item-services__text">
              We focus on ergonomics and meeting you where you work.
            </h3>
          </div>
          <div class="services__item item-services">
            <div class="item-services__icon">
              <img src="../assets/images/services/2.svg" alt="" />
            </div>
            <h2 class="item-services__title">Finance and consultancy</h2>
            <h3 class="item-services__text">
              Just type what's on your mind and we'll get you there.
            </h3>
          </div>
          <div class="services__item item-services item-services-green">
            <div class="item-services__icon">
              <img src="../assets/images/services/3.svg" alt="" />
            </div>
            <h2 class="item-services__title">Financial Services Consulting</h2>
            <h3 class="item-services__text">the quick fox jumps over the lazy dog</h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ServicesPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
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
  height: 100%;
  gap: 30px;
  flex-wrap: nowrap;
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
@media (max-width: 992px) {
  .services__column {
    flex-wrap: wrap;
    gap: unset;
  }
  .services__item {
    flex: 0 1 48%;
    margin: 0 0 30px 0;
  }
}
@media (max-width: 670px) {
  .services__item {
    flex: 0 1 100%;
    margin: 0 15px 15px 15px;
  }
}
</style>
