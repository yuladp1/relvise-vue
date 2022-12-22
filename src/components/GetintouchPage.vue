<template>
  <section class="page__getintouch getintouch">
    <div class="getintouch__container _container">
      <div class="getintouch__header header-block">
        <h2 class="header__block-title">Get In Touch</h2>
        <h3 class="header__block-text">
          Problems trying to resolve the conflict between the two major realms of
          Classical physics: Newtonian mechanics
        </h3>
      </div>
      <div class="getintouch__items">
        <div class="getintouch__item">
          <div class="getintouch__icon">
            <img src="../assets/images/getintouch/1.svg" alt="" />
          </div>
          <div class="getintouch__emails">
            <a href="mailto:georgia.young@example.com">georgia.young@example.com</a>
            <a href="mailto:georgia.young@ple.com">georgia.young@ple.com</a>
          </div>
          <div class="getintouch__label">Get Support</div>
          <a href="" class="getintouch__button">Submit Request</a>
        </div>
        <div class="getintouch__item">
          <div class="getintouch__icon">
            <img src="../assets/images/getintouch/3.svg" alt="" />
          </div>
          <div class="getintouch__emails">
            <a href="mailto:georgia.young@example.com">georgia.young@example.com</a>
            <a href="mailto:georgia.young@ple.com">georgia.young@ple.com</a>
          </div>
          <div class="getintouch__label">Get Support</div>
          <a href="" class="getintouch__button">Submit Request</a>
        </div>
        <div class="getintouch__item">
          <div class="getintouch__icon">
            <img src="../assets/images/getintouch/1.svg" alt="" />
          </div>
          <div class="getintouch__emails">
            <a href="mailto:georgia.young@example.com">georgia.young@example.com</a>
            <a href="mailto:georgia.young@ple.com">georgia.young@ple.com</a>
          </div>
          <div class="getintouch__label">Get Support</div>
          <a href="" class="getintouch__button">Submit Request</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "GetintouchPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.getintouch {
  padding: 80px 0 136px 0;
}

.getintouch__header {
  margin: 0 0 80px 0;
}
.getintouch__items {
  margin: 0 -15px;
  display: flex;
  align-items: center;
}
.getintouch__item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex: 0 1 33.3333%;
  background: white;
  padding: 50px 15px;
}
.getintouch__item > *:not(:last-child) {
  padding-bottom: 15px;
}
.getintouch__emails {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  text-align: center;
  color: #252b42;
  text-decoration: none;
}
.getintouch__emails > a {
  color: #252b42;
}
.getintouch__emails > *:hover {
  text-decoration: underline;
}
.getintouch__label {
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
  text-align: center;
  letter-spacing: 0.1px;
  color: #252b42;
}
.getintouch__button {
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  text-align: center;
  letter-spacing: 0.2px;
  color: #ff7b47;
  border: 1px solid #ff7b47;
  border-radius: 5px;
  padding: 10px 20px;
  transition: all 0.3s ease 0.2s;
}
.getintouch__button:hover {
  color: white;
  background-color: #ff7b47;
}
@media (max-width: 992px) {
  .getintouch {
    padding: 40px 0 40px 0;
  }
  .getintouch__items {
    flex-direction: column;
  }
  .getintouch__item {
    min-width: 100%;
  }
}
</style>
