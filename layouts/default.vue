<template>
  <div>
    <div class="navbar-fixed">
      <nav class="white" role="navigation">
        <div class="nav-wrapper container">
          <nuxt-link to="#top">
            <img src="~/assets/integra_logo.png" class="brand-logo" alt />
          </nuxt-link>

          <ul class="right hide-on-med-and-down">
            <li>
              <nuxt-link to="#about">О компании</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#features">Преимущества</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#service">Услуги</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#cert">Сертификаты</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#contacts">Контакты</nuxt-link>
            </li>
          </ul>

          <nuxt-link to="#" data-target="nav-mobile" class="sidenav-trigger">
            <i class="material-icons">menu</i>
          </nuxt-link>
        </div>
      </nav>
    </div>
    <ul class="sidenav" id="nav-mobile">
      <li><nuxt-link to="#top">            <img src="~/assets/integra_logo.png" class="brand-logo" alt />
</nuxt-link></li>
      <li>
        <nuxt-link to="#about">О компании</nuxt-link>
      </li>
      <li>
        <nuxt-link to="#features">Преимущества</nuxt-link>
      </li>
      <li>
        <nuxt-link to="#service">Услуги</nuxt-link>
      </li>
      <li>
        <nuxt-link to="#cert">Сертификаты</nuxt-link>
      </li>
      <li>
        <div class="divider"></div>
      </li>
      <li>
        <nuxt-link to="#contacts">Контакты</nuxt-link>
      </li>
    </ul>
    <main>
      <nuxt />
    </main>
    <footer class="page-footer blue darken-4">
      <div class="container" id="contacts">
        <div class="row">
          <div class="col">
            <h5 class="white-text">Контакты</h5>
            <p class="grey-text">Офис компании ООО "Интегра" в Санкт-Петербурге:</p>
            <ul>
              <li class="grey-text">190020, Санкт-Петербург, Лифляндская улица, дом 1</li>
              <li>
                <a href="tel:+79215797956">Телефон: +7 812 565 30 65</a>
              </li>
              <li>
                <a href="mailto:zaharov@integraelec.ru">E-mail: zaharov@integraelec.ru</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-copyright">
        <div class="container">
          <p class="grey-text right-align">
            Made with 💗 by
            <a href="https://github.com/frankieksai">Frankie Ksai</a>
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import M from "materialize-css";

export default Vue.extend({
  mounted() {
    // M.autoinit()
    M.AutoInit();
  }
});
</script>
<style scoped>
nav ul a,
nav .brand-logo {
  color: #444;
}
img {
  max-width: 100%;
  max-height: 100%;
}
</style>
