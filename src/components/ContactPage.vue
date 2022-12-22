<template>
  <section class="page__contact contact">
    <div class="contact__container _container">
      <div class="contact__body">
        <div class="contact__content">
          <h4 class="contact__title">Consulting Agency For Your Business</h4>
          <div class="contact__text">the quick fox jumps over the lazy dog</div>
        </div>
        <a href="contact__button" class="contact__button">Contact Us</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.contact__body {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 40px 38px 40px 0;
  background: #fafafa;
}
.contact__content {
  text-align: left;
  padding-right: 20px;
}
.contact__content > *:not(:last-child) {
  margin-bottom: 10px;
}
.contact__title {
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  letter-spacing: 0.1px;
  color: #252b42;
}
.contact__text {
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  color: #737373;
}
.contact__button {
  background: #ff7b47;
  border-radius: 5px;
  padding: 15px 40px;
  color: white;
  display: flex;
  align-items: center;
  transition: background-color 0.3s ease 0.2s;
}
.contact__button:hover {
  background: rgb(160, 62, 5);
}
@media (max-width: 723px) {
  .contact__body {
    padding: 20px;
    justify-content: center;
  }
  .contact__body > *:not(:last-child) {
    padding-bottom: 10px;
  }
  .contact__title {
    text-align: center;
  }
  .contact__text {
    text-align: center;
  }
  .contact__button {
    flex-basis: 80%;
    justify-content: center;
  }
}
</style>
