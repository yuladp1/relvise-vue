<template>
  <div class="page__clients clients">
    <div class="clients__container _container">
      <div class="clients__items">
        <div class="clients__item">
          <img src="../assets/images/clients/1.png" alt="" />
        </div>

        <div class="clients__item">
          <img src="../assets/images/clients/2.png" alt="" />
        </div>

        <div class="clients__item">
          <img src="../assets/images/clients/3.png" alt="" />
        </div>

        <div class="clients__item">
          <img src="../assets/images/clients/4.png" alt="" />
        </div>

        <div class="clients__item">
          <img src="../assets/images/clients/5.png" alt="" />
        </div>

        <div class="clients__item">
          <img src="../assets/images/clients/6.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ClientsPage",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.page__clients {
  margin: 0 0 10px 0;
}

.clients {
  padding: 50px 0;
}
.clients__items {
  display: flex;
  align-items: center;
  justify-content: center;

  flex-wrap: wrap;
}
.clients__item > img {
  max-width: 100%;
}

.clients__item {
  text-align: center;
  flex: 0 1 16.6667%;
  padding: 8px 15px;
  min-width: 140px;
}
</style>
