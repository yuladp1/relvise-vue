<template>
  <section class="page__whoweare whoweare">
    <div class="whoweare__wrapper _container">
      <div class="whoweare__header header-block">
        <h2 class="header__block-title">Who We Are</h2>
        <h3 class="header__block-text">
          Problems trying to resolve the conflict between the two major realms <br />
          of Classical physics: Newtonian mechanics
        </h3>
      </div>
      <div class="whoweare__body">
        <div class="whoweare__video">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/2uZYKcKHgU0"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <div class="whoweare__content">
          <div class="whoweare__header-content header-block">
            <h2 class="header__block-title">Most trusted in our field</h2>
            <h3 class="header__block-text">
              Most calendars are designed for teams. Slate is designed for freelancers who
              want a simple way to plan their schedule.
            </h3>
          </div>
          <div class="whoweare__items">
            <div class="whoweare__item item-whoweare">
              <div class="item-whoweare__icon">
                <img src="../assets/images/whoweare/1.svg" alt="" />
              </div>
              <div class="item-whoweare__body">
                <div class="item-whoweare__title">
                  the quick fox jumps over the lazy dog
                </div>
                <div class="item-whoweare__text">Things on a very small scale ...</div>
              </div>
            </div>
            <div class="whoweare__item item-whoweare">
              <div class="item-whoweare__icon">
                <img src="../assets/images/whoweare/2.svg" alt="" />
              </div>
              <div class="item-whoweare__body">
                <div class="item-whoweare__title">
                  the quick fox jumps over the lazy dog
                </div>
                <div class="item-whoweare__text">Things on a very small scale ...</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "WhowearePage",
};
</script>

<style scoped>
.whoweare {
  padding: 80px 0 130px 0;
  background-color: white;
}
@media (max-width: 950px) {
  .whoweare {
    padding-bottom: 20px;
  }
}
.whoweare__header {
  margin: 0 0 100px 0;
}
.whoweare__body {
  display: flex;
}
@media (max-width: 950px) {
  .whoweare__body {
    flex-direction: column-reverse;
  }
}
.whoweare__video {
  flex: 0 0 57%;
  position: relative;
  padding: 0 0 42.25% 0;
}
@media (max-width: 950px) {
  .whoweare__video {
    padding: 0 0 57% 0;
  }
  .whoweare__video > iframe {
    padding: 50px 0 0 0;
  }
}
.whoweare__video > iframe {
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  object-fit: cover;
}
.whoweare__header {
  margin: 0 0 100px 0;
}
@media (max-width: 950px) {
  .whoweare__header {
    margin: 0 0 40px 0;
  }
}
.whoweare__header-content {
  text-align: left;
  margin: 0 0 50px 0;
}
.whoweare__content {
  flex: 1 1 auto;
  padding: 20px 0 0 121px;
}

@media (max-width: 1080px) {
  .whoweare__content {
    flex: 1 1 auto;
    padding: 0 0 0 50px;
  }
}
@media (max-width: 950px) {
  .whoweare__content {
    padding: 20px;
  }
}
.whoweare__items {
  display: flex;
  flex-direction: column;
}
.whoweare__item {
  display: flex;
}
.whoweare__item:not(:last-child) {
  padding: 0 0 30px 0;
}
.item-whoweare__icon {
  flex: 0 0 32px;
}
.item-whoweare__body {
  flex: 1 1 auto;
  padding: 0 0 0 20px;
  text-align: left;
}
.item-whoweare__title {
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.1px;
  color: #252b42;
  padding-bottom: 5px;
}

.item-whoweare__text {
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  color: #737373;
}
</style>
