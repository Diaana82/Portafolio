<template>
  <header class="home">
      <section class="txt-header">
        <h1>¡Hola mi nombre es Diana!</h1>
        <h3>Soy Desarroladora web</h3>
      </section>
    </header>
    <section class="container-introduction">
        <div>
          <h1 class="">sobre mi</h1>
          <p class="">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Minus libero vitae, enim eum
            iste eos. In voluptate, ad aut culpa omnis accusantium assumenda consequatur, voluptatum
            voluptatibus pariatur officia maxime similique!
          </p>
          </div>
    </section>
    <div>
      <section class="project">
              <div class="item-1">
                <h1 class="info-title">MI PORYECTO</h1>
                <p class="info-subtitle">Lorem ipsum dolor sit amet consectetur adipisicing
                   elit. Dolorem illo voluptas iure obcaecati cumque. Culpa libero ratione,
                    molestias eligendi vero dolorem nostrum incidunt officia, quae illo
                     voluptatibus, praesentium id? Et.</p>
              </div>
              <div class="item-2">
                <img class="imagen" src="" alt="Logo">
              </div>
        </section>
        <section class="tecno">
          <h1>Tecnologías</h1>
          <div>
            <img src="" alt="vue">
            <img src="" alt="js">
            <img src="" alt="html">
            <img src="" alt="css">
          </div>
        </section>
        <section class="buttonn">
          <input type="button" value="¡Contáctame!">
        </section>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomeView',
});
</script>

<style>
.home{
  width: 100%;
  height: 450px;
  position: relative;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  background-color: darkgrey;
}
.container-introduction{
  background-color: hotpink;
}
.project{
  background-color: lawngreen;
}
.item-1{
  grid-area: a;
}
.item-2{
  grid-area: b;
  justify-content: center;
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
  background-color: aqua;
}
.buttonn{
  background-color: lightgreen;
}
</style>
