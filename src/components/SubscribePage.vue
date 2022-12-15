<template>
  <section class="page__subscribe subscribe">
    <div class="subscribe__container _container">
      <div class="subscribe__body">
        <h4 class="subscribe__title">Subscribe For Latest Newsletter</h4>
        <form class="subscribe__form" v-on:submit.prevent="handleSubmit">
          <input
            class="subscribe__input"
            type="email"
            required
            placeholder="your email"
            v-model="email"
          />
          <button class="subscribe__button" type="submit">Submit</button>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SubscribePage",
  created() {},
  data() {
    return {
      email: "",
    };
  },
  props: {},
  methods: {
    handleSubmit() {
      console.log(this.email);
    },
  },
};
</script>

<style scoped>
/* ------subscribe--------*/
.subscribe {
  position: relative;
  z-index: 3;
  padding: 0 0 20px 0;
}
.subscribe::before {
  content: "";
  background: #252b42;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 77px;
}
.subscribe__body {
  background-color: #17213c;
  display: flex;
  align-items: stretch;
  justify-content: space-between;
  padding: 50px 30px;
  margin: 0 30px;
  position: relative;
}

@media (max-width: 950px) {
  .subscribe__body {
    flex-direction: column;
    margin: 0 0;
  }
}
.subscribe__title {
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  letter-spacing: 0.1px;
  color: #ffffff;
  text-align: left;
  flex: 0 1 50%;
  max-width: 266px;
}
@media (max-width: 950px) {
  .subscribe__title {
    max-width: 100%;
    padding-bottom: 20px;
  }
}
.subscribe__form {
  flex: 0 1 50%;
  display: flex;
  align-items: stretch;
  justify-content: flex-end;
}
@media (max-width: 950px) {
  .subscribe__form {
    max-width: 70%;
  }
}
.subscribe__input {
  flex: 1 1 auto;
  font-weight: 400;
  font-size: 14px;
  line-height: 28px;
  letter-spacing: 0.2px;
  color: #737373;
  padding-left: 20px;
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
}
.subscribe__button {
  color: white;
  background: #ff7b47;
  border: 1px solid #e6e6e6;
  border-radius: 0px 5px 5px 0px;
  padding: 15px 22px;
}
</style>
