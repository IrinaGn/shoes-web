<template>
  <div class="home">
    <img class="logo" alt="logo" src="../assets/shoemaker-logo.png" />
    <div class="head">
      <div class="parent">
        <div class="child">
          <h3>Мастерская</h3>
          <h1>Shoesmakermd</h1>
          <p>
            Профессиональный сервис, оказывающий услуги по уходу, косметической
            реставрации и ремонту обуви.
          </p>
          <button class="btn-form btn-red">Узнать цену</button>
        </div>
      </div>
      <div class="header-image">
        <!-- <div class="header-i"> -->
        <!-- <img class="header-img" src="../img/repair.jpg" alt="" /> -->
        <!-- </div> -->
      </div>
    </div>
    <Brands msg="Welcome to Your Vue.js App" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <ClientForm msg="Узнать цену" />
    <AppFooter />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Brands from "@/components/Brands.vue";
import AppFooter from "@/layout/AppFooter.vue";
import ClientForm from "@/components/ClientForm.vue";

export default {
  name: "HomeView",
  components: {
    // HelloWorld,
    Brands,
    AppFooter,
    ClientForm,
  },
};
</script>

<style lang="scss">
.logo {
  width: 10%;
}
.head {
  display: grid;
  grid-template-columns: 1.5fr 2fr;
  // display: flex;
  // justify-content: space-around;
  margin-left: 10%;
  margin-right: 10%;
}
.btn-form {
  border-radius: 6px;
  color: #fff;
  letter-spacing: 0.05em;
  padding: 13px 29px;
  width: 50%;
}
.btn-red {
  background: #aa2c18;
  border: 2px solid #aa2c18;
}
.btn-red:hover {
  background: #a30000;
}
.header-image {
  display: flex;
  justify-content: flex-end;

  background-image: url(../img/repair.jpg);
  background-position: center center;
  background-size: cover;
  height: 550px;
}
.header-img {
  width: 90%;
}
.parent {
  // background: gray;
  // height: 300px;
  width: 100%;
  position: relative;
}

.child {
  // background: orange;
  position: absolute;
  top: 30%;
  left: 0;
  right: 10%;
  // right: 0;
  text-align: left;
  // margin: -50px 0 0 -50px;
}
@media screen and (max-width: 600px) {
  .logo {
    width: 30%;
  }
  .head {
    // flex-direction: column;
    grid-template-columns: 1fr;
    // margin-bottom: 100px;
    height: 250px;
  }
  .child {
    top: 5%;
    left: 0;
    right: 0;
  }
  .header-image {
    display: none;
  }
}
@media screen and (max-width: 768px) {
  .child {
    // top: 30%;
    // right: 0;
    font-size: 85%;
    text-align: center;
  }
  .head {
    margin-left: 0;
    margin-right: 0;
  }
}
@media (min-width: 2000px) {
  .header-image {
    height: 800px;
  }
}
</style>
