<template>
  <nav class="nav-bar">
    <div>
      <img src="" alt="logo">
    </div>

    <div class="nav-bar__right">
      <a href="">Say hello</a>
    </div>
  </nav>
  <router-view/>
  <footer>
    <div>
      <img src="" alt="logo">
    </div>
  <div class="main-footer__phrase">
    <p>"If you think good architecture is expensive, try bad architecture."</p>
  </div>

  <div class="main-footer__social-media">
    <a href="#"><Icon icon="el:github-text" /> github</a>
    <a href="#"><Icon icon="eva:linkedin-fill" /> linkedin</a>
  </div>
  <div class="grupo-2">
    <small>&copy; 2022 <b> Diaana82</b></small>
  </div>
  </footer>
</template>

<style lang="scss">
*{
  margin: auto;
}
</style>
<style>
.nav-bar{
  background-color: blueviolet;
}
footer{
  background-color: crimson;
}
</style>
