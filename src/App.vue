<template>
  <div :class="theme === 'theme--light' ? 'theme--light' : 'theme--dark'">
    <nav class="nav-bar">
      <div>
        <img class="nav-img" src="./assets/media/icono.png" alt="logo" />
      </div>
      <div class="nav-txt">
        <a href="">Say hello</a>
      </div>
    </nav>
    <router-view />
    <footer>
      <div>
        <img class="footer-img" src="./assets/media/icono.png" alt="logo" />
      </div>
      <div class="main-footer__phrase">
        <p class="text-footer">"If you think good architecture is expensive,
        try bad architecture".<br/>Hecho por mi.</p>
      </div>
      <div class="main-footer__social-media">
        <div class="linkedin">
          <a href="https://www.linkedin.com/in/diana-cristina-pati%C3%B1o-ramirez-172340243/">
          <iconify-icon style="color:#000" icon="akar-icons:linkedin-v1-fill">|</iconify-icon>
          </a>
        </div>
        <div class="github">
          <a href="https://github.com/Diaana82">
          <iconify-icon style="color:#000" icon="ant-design:github-outlined">|</iconify-icon>
          </a>
        </div>
        <div class="whatsapp">
          <a href="tel:+57 3135374647">
          <iconify-icon style="color:#000" icon="simple-icons:whatsapp">|</iconify-icon>
          </a>
        </div>
        <div class="instagram">
          <a style="color:#000" href="https://www.instagram.com/dianacristina_pati/">
          <iconify-icon icon="ri:instagram-fill">.</iconify-icon>
          </a>
        </div>
      </div>
      <button class="boton" @click="cambiarT()">Cambiar Tema</button>
      <div class="grupo-2">
        <small>&copy; 2022 <b> Diaana82</b></small>
      </div>
    </footer>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      theme: 'theme--light',
    };
  },
  methods: {
    cambiarT() {
      // console.log(this.theme);
      this.theme = this.theme === 'theme--dark' ? 'theme--light' : 'theme--dark';
    },
  },
};
</script>

<style lang="scss">
@use "./assets/styles/main.scss";
// navbar
.nav-bar {
  position: absolute;
  display: flex;
  justify-content: space-between;
  padding: 10px 20px;
  background-color: var(--color-background-2);
  z-index: 3;
  width: 100%;
}
.nav-img {
  width: 30px;
  height: 30px;
  object-position: left;
  align-items: flex-start;
}
.nav-txt a {
  object-position: right;
  align-items: flex-start;
  text-decoration: none;
  color: rgb(0, 0, 0);
}
//Footer
footer {
  background-color: var(--color-background-2);
  justify-content: center;
  text-align: center;
  color: var(color-text-2);
  padding: 3%;
}
.footer-img{
  width: 10%;
  height: 10%;
  margin: 0%;
}
.text-footer{
  padding: 3%;
}
.main-footer__social-media {
  display: flex;
  justify-content: space-evenly;
  padding: 3%;
}
.linkedin{
  font-size: 30px;
}
.github{
  font-size: 30px;
}
.whatsapp{
  font-size: 30px;
}
.instagram{
  font-size: 30px;
}
.boton{
  background-color: #000;
  border: none;
  padding: 1%;
  color: #fff;
}
</style>
