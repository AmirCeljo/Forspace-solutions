<!-- eslint-disable -->
<template>
  <nav>
    <router-link to="/">{{ $t("home") }}</router-link> |
    <router-link to="/news">{{ $t("news") }}</router-link> |
    <router-link to="/about">{{ $t("about") }} </router-link> |
    <router-link to="/products">{{ $t("products") }}</router-link> |
    <router-link to="/services">{{ $t("services") }}</router-link> |
    <router-link to="/forspace-preview">{{ $t("preview") }}</router-link> |
    <router-link to="/contact">{{ $t("contact") }}</router-link> |
    <router-link to="/promo">{{ $t("promo") }}</router-link>
  </nav>
  <router-view />
</template>
<style lang="scss">
@import "./styles/variables.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $primary-blue;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
  h1 {
    color: $primary-blue;
  }
}
</style>
