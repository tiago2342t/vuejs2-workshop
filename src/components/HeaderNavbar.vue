<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#"><img src="../assets/img/logo-blue.png" alt="Logo de PeakU"></a>
    <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button> -->

    <div class="collapse navbar-collapse" id="navbarSupportedContent" style="display:none;">
      <ul class="navbar-nav ml-md-auto align-items-md-center">
        <li class="nav-item active">
          <a class="nav-link" href="#">Empleos <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Bootcamp</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Sobre nosotros</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-toggle="dropdown" aria-expanded="false">
            Para profesionales
          </a>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Inicio</a>
            <a class="dropdown-item" href="#">Empleos</a>
            <a class="dropdown-item" href="#">Cursos y retos</a>
            <a class="dropdown-item" href="#">Preguntas</a>
            <a class="dropdown-item" href="#">Profesores</a>
            <a class="dropdown-item" href="#">Bootcamp</a>
          </div>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-toggle="dropdown" aria-expanded="false">
            Para empresas
          </a>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Inicio</a>
            <a class="dropdown-item" href="#">Publicar empleo</a>
            <a class="dropdown-item" href="#">Nuestro proceso</a>
            <a class="dropdown-item" href="#">Precios</a>
            <a class="dropdown-item" href="#">Pruebas Online</a>
            <a class="dropdown-item" href="#">Nómina</a>
            <a class="dropdown-item" href="#">Blog</a>
            <a class="dropdown-item" href="#">Comercial</a>
            <a class="dropdown-item" href="#">Calculadora de salarios</a>
          </div>
        </li>
        <li class="nav-item">
            <div class="d-flex align-items-center justify-content-center lang-btn">
              <i class="bi bi-globe2 mr-1"></i>
              <span>Español</span>
            </div>
        </li>
        <li class="nav-item">
            <div class="d-flex align-items-center justify-content-center bell-btn">
              <i class="bi bi-bell"></i>
            </div>
        </li>
        <li class="nav-item">
            <div class="d-flex align-items-center justify-content-center user-btn">
              <i class="bi bi-person mr-1"></i>
              <span>User</span>
            </div>
        </li>
      </ul>
      <!-- <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
      </form> -->
    </div>
  </nav>
</template>

<script setup>
// export default {
//     name: 'HeaderNavbar'
// }
</script>

<style scoped>
li.nav-item {
  padding: 0 0.5rem;
}

.lang-btn {
  border: 1px solid rgb(177, 176, 176);
  padding: 0.2rem 0.8rem;
  border-radius: 5px;
}

.lang-btn i, .lang-btn span {
  color: gray;
  transition: all 0.2s ease-in;
}

.lang-btn:hover i, .lang-btn:hover span {
  color: black;
}

.bell-btn {
  padding: 0.1rem 0.5rem;
}

.user-btn {
    padding: 0.3rem 0.8rem;
}

.bell-btn i {
  color: black;
  font-size: 1.5rem;
}

.user-btn i {
  background-color: #343a40;
  color: white;
  padding: 0 0.3rem;
  font-size: 1.25rem;
  border-radius: 50%;
}

.bell-btn:hover, .user-btn:hover {
  background-color: rgb(233, 231, 231);
  border-radius: 5px;
}
</style>