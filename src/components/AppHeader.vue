<template>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg">
    <!-- Container wrapper -->
    <div class="container">
      <!-- Toggle button -->
      <button
        class="navbar-toggler"
        type="button"
        data-mdb-toggle="collapse"
        data-mdb-target="#navbarButtonsExample"
        aria-controls="navbarButtonsExample"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <em class="fas fa-bars"></em>
      </button>

      <!-- Collapsible wrapper -->
      <div class="collapse navbar-collapse" id="navbarButtonsExample">
        <!-- Left links -->
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link" href="#">
              Espace de travail
              <em class="fas fa-angle-down"></em>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              Récent
              <em class="fas fa-angle-down"></em>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              Favoris
              <em class="fas fa-angle-down"></em>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              Modèles
              <em class="fas fa-angle-down"></em>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link btn__creer" href="#"> Créer </a>
          </li>
        </ul>
      </div>
      <!-- Collapsible wrapper -->
    </div>
    <!-- Container wrapper -->
  </nav>
  <!-- Navbar -->
  <!-- <router-link to="/">Mis paneles</router-link> -->
</template>

<script>
export default {
  name: "app-header",
};
</script>

<style lang="scss" scoped>
nav {
  background-color: #0d6b9c;
  height: 50px;
  .collapse {
    .nav-link {
      color: #fbfbfb;
      font-weight: lighter;
      font-size: 14px;
      letter-spacing: 0.5px;
      margin-right: 15px;
    }
    .nav-link:hover {
      background-color: #1a86c2;
      border-radius: 5px;
    }
    .btn__creer {
      text-transform: none;
      background-color: #1a86c2;
      border-radius: 5px;
    }
  }
}
</style>
