<template>
<div class="container text-center">
  <div class="row">
  <div class="col">
    <div class="card" style="width: 18rem;">
      <img src="../assets/media/ies.png" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">IES CINOC</h5>
        <p class="card-text">Técnico Profesional en soporte
          y operaciones de sistemas infromaticos.
          <br/> 2021-2022</p>
        <a href="#" class="btn btn-primary">IES CINOC</a>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card" style="width: 18rem;">
      <img src="../assets/media/prosper.png" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Prospercity</h5>
        <p class="card-text">Desarrolladora web<br/>2022</p>
        <a href="https://www.prospercity.co/" class="btn btn-primary">Prospercity</a>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card" style="width: 18rem;">
      <img src="../assets/media/linkedai.png" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">LinkedAi</h5>
        <p class="card-text">Labeler<br/>Apoyo al equipo de creación de
          algoritmos de machine learning catalogando piezas de
          imagenes y datos<br/>
          2022</p>
        <a href="https://linkedai.co/" class="btn btn-primary">LinkedAi</a>
      </div>
    </div>
  </div>
  </div>
</div>
</template>

<style>
.experience-1{
  grid-area: a;
}
.experience-2{
  grid-area: b;
}
.experience-3{
  grid-area: c;
}
.card-img-top{
  margin-top: 5%;
  margin-bottom: 5%;
  margin-left: 15%;
  margin-right: 10%;
  width: 200px;
  height: 200px;
}
.card{
  background-color: var(--color-background-1);
  text-align: center;
  padding: 5%;
  gap: 5%;
}
.experience{
  padding: 3%;
  background-color: var(--color-background-2);
  /* display:grid;
  grid-template-areas:
  "a"
  "b"
  "c"; */
}
/* @media (min-width: 600px){
  .experience{
    grid-template:
    "a b"
    " c ";
  }
} */
</style>
