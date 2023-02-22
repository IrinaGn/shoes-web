<template>
  <nav>
    <router-link to="/">Главная</router-link> |
    <router-link to="/about">О нас</router-link> |
    <!-- <router-link to="/contacts">Контакты</router-link> -->
  </nav>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #000000;

    &.router-link-exact-active {
      color: #aa2c18;
      font-size: larger;
    }
  }
}
</style>
