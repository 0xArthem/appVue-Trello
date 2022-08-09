<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-mdb-toggle="collapse"
        data-mdb-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <router-link to="/">
            <a class="nav-link" href="#">
              <em class="fab fa-trello"></em>
              Tableau
              <em class="fas fa-angle-down"></em>
            </a>
          </router-link>
          <a class="nav-link" href="#">
            <em class="far fa-star"></em>
          </a>
          <a class="nav-link" href="#">Casca</a>
          <a class="nav-link" href="#">
            <em class="fas fa-lock"></em>
            Privé
          </a>
          <a class="nav-link" href="#">
            <em class="fas fa-user-plus"></em>
            Partager
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "app-header-down",
};
</script>

<style lang="scss" scoped>
nav {
  background-color: #2e91d5;
  box-shadow: none !important;
  .collapse {
    margin-left: 5%;
    .nav-link {
      font-size: 14px;
      color: #fbfbfb;
      background-color: #1a86c2;
      border-radius: 5px;
      margin-right: 10px;
      font-weight: lighter;
      .fa-user-plus {
        margin-right: 5px;
      }
      .fa-lock {
        margin-right: 5px;
      }
      .fa-trello {
        margin-right: 5px;
      }
      .fa-angle-down {
        margin-left: 5px;
      }
    }
  }
}
</style>
