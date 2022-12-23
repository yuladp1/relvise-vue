<template>
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

    <div class="practice__body">
      <div class="practice__column _container">
        <article class="practice__item item-practice">
          <div class="item-practice__content">
            <a href="" class="item-practice__link">
              <h4 class="item-practice__title">
                A single source <br />
                of truth
              </h4>
            </a>
            <div class="item-practice__text">
              Newton thought that light was made up of particles, but then it was
              discovered
            </div>
          </div>
          <a href="" class="item-practice__image _ibg">
            <img src="../assets/images/practice/1.jpg" alt="" />
          </a>
        </article>
        <article class="practice__item item-practice">
          <div class="item-practice__content">
            <a href="" class="item-practice__link">
              <h4 class="item-practice__title">Fastest way to organize</h4>
            </a>
            <div class="item-practice__text">
              “Quantum mechanics” is the description of the behaviour of matter
            </div>
          </div>
          <a href="" class="item-practice__image _ibg">
            <img src="../assets/images/practice/2.jpg" alt="" />
          </a>
        </article>
        <article class="practice__item item-practice">
          <div class="item-practice__content">
            <a href="" class="item-practice__link">
              <h4 class="item-practice__title">Fastest way to take action</h4>
            </a>
            <div class="item-practice__text">
              They describe a universe consisting of bodies moving
            </div>
          </div>
          <a href="" class="item-practice__image _ibg">
            <img src="../assets/images/practice/3.jpg" alt="" />
          </a>
        </article>
        <article class="practice__item item-practice">
          <div class="item-practice__content">
            <a href="" class="item-practice__link">
              <h4 class="item-practice__title">Work better together</h4>
            </a>
            <div class="item-practice__text">
              They finally obtained a consistent description of the behaviour
            </div>
          </div>
          <a href="" class="item-practice__image _ibg">
            <img src="../assets/images/practice/4.jpg" alt="" />
          </a>
        </article>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PracticePage",
};
</script>

<style scoped>
.practice {
  padding: 125px 0 80px 0;
}
.practice__header {
  margin: 0 0 45px 0;
}
.practice__body {
  margin: 0 -15px;
  display: flex;
  flex-wrap: wrap;
}
.practice__column {
  display: flex;
  padding: 0 15px;
  flex-wrap: wrap;
}
.practice__item {
  background-color: #fff;
  padding: 0 15px;
  flex: 0 1 25%;
}
@media (max-width: 1000px) {
  .practice__item {
    flex: 0 1 50%;
  }
}
@media (max-width: 670px) {
  .practice__item {
    flex: 0 1 100%;
  }
}
.item-practice {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.item-practice__content {
  padding: 30px;
}
.item-practice__link {
  display: inline-block;
}
.item-practice__link:hover {
  transform: scale(1.1);
  color: #0cbccc;
}
.item-practice__link:not(:last-child) {
  margin: 0 0 15px 0;
}
.item-practice__title {
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.1px;
  color: #252b42;
}
.item-practice__text {
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  color: #737373;
}
.item-practice__text:hover {
  color: black;
}
.item-practice__image {
  display: block;
  height: 138px;
  width: 100%;
  padding: 0 0 67% 0;
}
.item-practice__image > img {
  width: 100%;
  height: 100%;
}
</style>
