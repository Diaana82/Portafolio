<template>
  <header class="home">
      <section class="txt-header">
        <h1>Hi,I'm Diana!,<br/>FrontEnd developer</h1>
      </section>
    </header>
    <section class="container-introduction">
        <div class="about-me">
          <h1 class="title-description">About me</h1>
          <p>I am a web developer, I have been
             focused on the world of technology for about two years, I like to learn
             new things every day in order to improve my skills and offer new
              technologies to the industry.
          </p>
          </div>
    </section>
    <ExperienceComp />
    <div>
      <section class="project">
              <div class="item-1">
                <h1 class="info-title">My project</h1>
                <p class="info-subtitle">Dulces del campo es una tienda virtual
                    de productos a base de caña de azucar creados
                    para la facil distribucion de estos
                    productos y asi ayudar al campo colombiano.</p>
              </div>
              <div class="item-2">
                <img class="img-project" src="../assets/media/Logo-r.png" alt="Logo">
              </div>
        </section>
        <section class="tecno">
          <h1>Technologies</h1>
          <div class="tecno-logos">
            <iconify-icon style="font-size:50px" icon="logos:html-5"></iconify-icon>
            <iconify-icon style="font-size:50px" icon="logos:css-3"></iconify-icon>
            <iconify-icon style="font-size:50px" icon="logos:javascript"></iconify-icon>
            <iconify-icon style="font-size:50px" icon="logos:vue"></iconify-icon>
          </div>
        </section>
        <section class="button-container">
          <input class="buttonn" type="button" value="Contact me!">
        </section>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ExperienceComp from '@/components/experienceComp.vue';

export default defineComponent({
  name: 'HomeView',
  components: { ExperienceComp },
});
</script>

<style lang="scss">
//home
.home{
  width: 100%;
  height: 350px;
  position: relative;
  background: url(../assets/media/img-home.png);
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
.txt-header{
  position: absolute;
  color: #fff;
  text-align: center;
  left: 20%;
  right: 20%;
  top: 50%;
  bottom: 50%;
}
//about me
.container-introduction{
  background-color: var(--color-background-1);
  padding-bottom: 10%;
 padding-left: 10%;
  padding-right: 10%;
}
.about-me{
  text-align: center;
  margin-left: 10%;
  margin-right: 10%;
  color: var(--color-text-2)
}
.title-description{
  padding: 5%;
}
//project
.project{
  background-color: var(--color-background-1);
  padding: 5%;
}
.item-1{
  grid-area: a;
  text-align: center;
  margin-left: 5%;
  margin-right: 5%;
  color: var(--color-text-2)
}
.info-title{
  padding: 5%;
}
.item-2{
  grid-area: b;
  justify-content: center;
  margin: auto;
  text-align: center;
}
.img-project{
  width: 40%;
  height: 40%;
}
.project{
  display: grid;
  grid-template-columns: repeat(2,1fr);
  grid-template-rows: auto auto;
  grid-template-areas:
    "a a"
    "b b";
}
@media (min-width: 600px) {
  .project {
    grid-template-areas:
    "a  b";
  }
}
.tecno{
  background-color: var(--color-background-2);
  text-align: center;
  color: var(--color-text-2);
  padding: 5%;
}
.tecno-logos{
  display: flex;
  justify-content: space-evenly;
  padding: 6%;
}
.button-container{
  background-color: var(--color-background-1);
  text-align: center;
  padding: 10%;
}
.buttonn{
  background-color: var(--color-background-button);
  border: none;
  color: var(--color-text-2);
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 20px;
}
</style>
