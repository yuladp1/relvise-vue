<template>
  <footer class="footer">
    <div class="footer__top">
      <div class="footer__container _container">
        <div class="footer__main">
          <div class="footer__column">
            <div class="footer__label">Company Info</div>
            <nav class="footer__menu menu-footer">
              <ul class="menu-footer__list">
                <li class="menu-footer__item"><a href="">About Us</a></li>
                <li class="menu-footer__item"><a href="">Carrier</a></li>
                <li class="menu-footer__item"><a href="">We are hiring</a></li>
                <li class="menu-footer__item"><a href="">Blog</a></li>
              </ul>
            </nav>
          </div>
          <div class="footer__column">
            <div class="footer__label">Company Info</div>
            <nav class="footer__menu menu-footer">
              <ul class="menu-footer__list">
                <li class="menu-footer__item"><a href="">About Us</a></li>
                <li class="menu-footer__item"><a href="">Carrier</a></li>
                <li class="menu-footer__item"><a href="">We are hiring</a></li>
                <li class="menu-footer__item"><a href="">Blog</a></li>
              </ul>
            </nav>
          </div>
          <div class="footer__column">
            <div class="footer__label">Legal</div>
            <nav class="footer__menu menu-footer">
              <ul class="menu-footer__list">
                <li class="menu-footer__item"><a href="">About Us</a></li>
                <li class="menu-footer__item"><a href="">Carrier</a></li>
                <li class="menu-footer__item"><a href="">We are hiring</a></li>
                <li class="menu-footer__item"><a href="">Blog</a></li>
              </ul>
            </nav>
          </div>
          <div class="footer__column">
            <div class="footer__label">Resources</div>
            <nav class="footer__menu menu-footer">
              <ul class="menu-footer__list">
                <li class="menu-footer__item"><a href="">About Us</a></li>
                <li class="menu-footer__item"><a href="">Carrier</a></li>
                <li class="menu-footer__item"><a href="">We are hiring</a></li>
                <li class="menu-footer__item"><a href="">Blog</a></li>
              </ul>
            </nav>
          </div>
          <div class="footer__column">
            <div class="footer__label">Get In Touch</div>
            <div class="footer__contacts">
              <a class="footer__contacts-itemphone" href="tel:4805550103"
                >(480) 555-0103</a
              >
              <a class="footer__contacts-adress" href=""
                >4517 Washington Ave. Manchester, Kentucky 39495</a
              >
              <a class="footer__contacts-mail" href="mailto:debra.holt@example.com"
                >debra.holt@example.com</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-social">
      <div class="footer-social__container _container">
        <div class="footer-social__main-wrapper">
          <div class="footer-social__main">
            <h4 class="footer-social-text">
              Made With Love By Figmaland All Right Reserved
            </h4>
            <div class="footer-social__icons">
              <a href=""> <img src="../assets/images/footer-bottom/1.svg" alt="" /></a>
              <a href=""> <img src="../assets/images/footer-bottom/2.svg" alt="" /></a>
              <a href=""> <img src="../assets/images/footer-bottom/3.svg" alt="" /></a>
              <a href=""> <img src="../assets/images/footer-bottom/4.svg" alt="" /></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.footer__top {
  background-color: #17213c;
  color: white;
  padding-bottom: 50px;
}
footer__container {
  margin: 0 -15px;
}
.footer__main {
  display: flex;
  padding: 0 15px;
  flex-wrap: wrap;
}
.footer__column {
  flex: 0 1 16.667%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  min-width: 148px;
  margin-top: 50px;
}
.footer__column:last-child {
  flex: 0 1 33.334%;
}

.footer__label {
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.1px;
  padding-bottom: 10px;
}

.menu-footer__list {
  display: flex;
  justify-content: flex-start;
  flex-direction: column;
  align-items: flex-start;
}
.menu-footer__list > * {
  padding: 10px 0 0 0;
}
.menu-footer__item a {
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  letter-spacing: 0.2px;
  color: #ffffff;
}
.menu-footer__item a:hover {
  text-decoration: underline;
}
.footer__contacts {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.footer__contacts > a {
  margin: 12px 0 0 0;
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  color: white;
  padding-left: 34px;
}
.footer__contacts-itemphone {
  background: url("../assets/images/footer-top/1.svg") left no-repeat;
}
.footer__contacts-adress {
  background: url("../assets/images/footer-top/2.svg") left no-repeat;
  text-align: left;
}
.footer__contacts-mail {
  background: url("../assets/images/footer-top/3.svg") left no-repeat;
}
.footer-social__main-wrapper {
  margin: 0 -15px;
}
.footer-social__main {
  display: flex;
  justify-content: space-between;
  padding: 20px 30px;
  align-items: center;
}
.footer-social-text {
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
  color: #737373;
  padding-right: 15px;
}
.footer-social__icons {
  display: flex;
}
.footer-social__icons > a:not(:last-child) {
  padding: 0 20px 0 0;
}
@media (max-width: 950px) {
  .footer__column {
    flex: 0 1 25%;
  }
  .footer__column:last-child {
    flex: 0 1 100%;
  }
}
</style>
