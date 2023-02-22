<template>
  <section class="about">
    <div class="container">
      <h2 class="display-3">Подробнее о нас</h2>
      <h5 class="display-4 mt-4">Работаем с 2015 года</h5>
      <p class="lead">Мастерская Мастерская Shoesmaker</p>
      <p class="lead">
        Профессиональный сервис, оказывающий услуги по уходу, косметической
        реставрации и ремонту обуви.
      </p>
    </div>
    <div class="header-image">
      <!-- <img src="" alt="" /> -->
    </div>
    <AppFooter />
  </section>
</template>
<script>
import AppFooter from "@/layout/AppFooter.vue";

export default {
  name: "HomeView",
  components: {
    AppFooter,
  },
};
</script>

<style lang="scss" scoped>
.header-image {
  display: flex;
  justify-content: flex-end;

  background-image: url(../img/office.jpg);
  background-position: center center;
  background-size: cover;
  height: 550px;
  margin: 5% 0 5% 0;
}
</style>
