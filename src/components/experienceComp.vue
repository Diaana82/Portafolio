<template>
  <section class="card-expe">
    <h1>Experiencia</h1>
  </section>
  <section class="experiencia">
    <div class="card" style="width: 18rem;">
    <img src="../assets/media/ies.png" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">IES CINOC</h5>
      <p class="card-text">Professional technician in support and
        operations of computer systems<br/>2021-2022</p>
      <a href="#" style=" background-color: var(--color-background-2);
      border-color: var(--color-background-2); color: var(--color-text-2);"
      class="btn btn-primary">Conocer sitio</a>
    </div>
    </div>

    <div class="card" style="width: 18rem;">
    <img src="../assets/media/prosper.png" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">PROSPERCITY</h5>
      <p class="card-text">Desarrolladora web<br/>2022</p>
      <a href="#" style=" background-color: var(--color-background-2);
      border-color: var(--color-background-2); color: var(--color-text-2);"
      class="btn btn-primary">Conocer sitio</a>
    </div>
    </div>

    <div class="card" style="width: 18rem;">
    <img src="../assets/media/linkedai.png" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">LINKEDAI</h5>
      <p class="card-text">Labeler<br/>2022</p>
      <a href="#" style=" background-color: var(--color-background-2);
      border-color: var(--color-background-2); color: var(--color-text-2);"
      class="btn btn-primary">Conocer sitio</a>
    </div>
    </div>
</section>
</template>

<style>
.card-expe{
  height: 150px;
  background-color: var(--color-background-2);
  text-align: center;
  padding-top: 5%;
}
.experiencia{
  display: grid;
  padding-left: 9%;
  padding-top:5%;
  padding-bottom: 5%;
  text-align: center;
  gap: 10%;
  grid-auto-rows: 25rem;
  grid-template-columns: repeat(auto-fill, minmax(14rem,1fr));
  background-color: var(--color-background-2);
}
.card{
  background-color: var(--color-background-1);
  color: var(--color-text-2);
}
.card-img-top{
  height: 150px;
  width: 150px;
  margin-left: 10%;
}
/* .row{
  background-color: aqua;
}
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
} */
</style>
