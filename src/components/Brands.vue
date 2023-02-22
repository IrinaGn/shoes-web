<template>
  <section class="brands">
    <div class="roww">
      <div class="container">
        <!-- <div> -->
        <h5>
          Мы ремонтируем обувь различных брендов. Вот некоторые из чаще
          встречающихся брендов.
        </h5>
        <!-- </div> -->
        <div class="brand-list">
          <img src="../img/brands/chanel.png" alt="" class="brand" />
          <img src="../img/brands/gucci.png" alt="" class="brand" />
          <img src="../img/brands/hermes.png" alt="" class="brand" />
          <img src="../img/brands/lv.png" alt="" class="brand" />
          <img src="../img/brands/lv.png" alt="" class="brand" />
          <img src="../img/brands/lv.png" alt="" class="brand" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.brands {
  background-color: #f0f0f0;
  // left: -10px;
  // position: absolute;
  margin: -8px;
  margin-top: 0;
  // padding-top: 10px;
  padding: 1%;
}
.roww {
  padding-top: 10px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.brand-list {
  display: flex;
  justify-content: space-around;

  // flex-basis: 25%;
}
.brand {
  margin: 20px;
  width: 10%;
}
.container {
  margin-left: 10%;
  margin-right: 10%;
  // margin: 10%;
}
.logo {
  width: 20%;
}
@media screen and (max-width: 600px) {
  .brand-list {
    flex-wrap: wrap;
  }
  .brand,
  .logo {
    width: 20%;
  }
}
</style>
