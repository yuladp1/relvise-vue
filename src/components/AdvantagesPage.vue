<template>
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
              <img src="../assets/images/advertise/1.svg" alt="" />
            </div>
            <div class="advantages__value">972 +</div>
            <div class="advantages__text">Consumer Products</div>
          </div>
        </div>

        <div class="advantages__column">
          <div class="advantages__item">
            <div class="advantages__icon">
              <img src="../assets/images/advertise/2.svg" alt="" />
            </div>
            <div class="advantages__value">181 +</div>
            <div class="advantages__text">Financial Services</div>
          </div>
        </div>
        <div class="advantages__column">
          <div class="advantages__item">
            <div class="advantages__icon">
              <img src="../assets/images/advertise/3.svg" alt="" />
            </div>
            <div class="advantages__value">98 %</div>
            <div class="advantages__text">Environmental</div>
          </div>
        </div>
        <div class="advantages__column">
          <div class="advantages__item">
            <div class="advantages__icon">
              <img src="../assets/images/advertise/4.svg" alt="" />
            </div>
            <div class="advantages__value">746 +</div>
            <div class="advantages__text">Business & Finance</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AdvantagesPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.advantages {
  padding: 80px 0 0 0;
}
.advantages__header {
  margin: 0 0 50px 0;
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
</style>
