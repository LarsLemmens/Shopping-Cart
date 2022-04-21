<template>
  <header
    class="text-center text-white d-flex masthead"
    v-bind:id="$attrs.page"
  >
    <div class="container my-auto">
      <nav
        class="navbar navbar-light navbar-expand-lg fixed-top"
        id="mainNav"
        style="position: absolute; height: 25%"
      >
        <div class="container">
          <h1>
            <a href="Home">
              <img
                src="./assets/img/vecteezy_dd-d-and-d-abstract-initial-monogram-letter-alphabet-logo_6150819.png"
                style="
                  /*opacity: &amp;;*/
                  opacity: 1;
                  color: var(--bs-yellow);
                " /></a
            >DreamDesk
          </h1>
          <h1 style="color: darkgoldenrod"></h1>
          <button
            data-bs-toggle="collapse"
            data-bs-target="#navbarResponsive"
            class="navbar-toggler navbar-toggler-right"
            type="button"
            aria-controls="navbarResponsive"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <i class="fa fa-align-justify"></i>
          </button>
          <div class="collapse navbar-collapse" id="navbarResponsive">
            <ul class="navbar-nav ms-auto">
              <li class="nav-item">
                <a class="nav-link" :href="$attrs.redirect + '#about'" style="color: white">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" :href="$attrs.redirect + '#services'" style="color: white"
                  >Services</a
                >
              </li>
              <li class="nav-item">
                <a class="nav-link" href="Builder" style="color: white"
                  >Desks</a
                >
              </li>
              <li class="nav-item"></li>
              <ul class="nav navbar-nav">
                <router-link
                  to="/"
                  tag="li"
                  v-if="!isAuthenticated"
                  class="nav-item"
                  active-class="active"
                >
                  <a @click="onLoginClicked" class="nav-link">Login</a>
                </router-link>
                <li v-if="isAuthenticated" class="li-pointer nav-item">
                  <div class="dropdown">
                    <button
                      class="btn btn-secondary dropdown-toggle"
                      type="button"
                      id="dropdownMenuButton"
                      data-toggle="dropdown"
                      aria-haspopup="true"
                      aria-expanded="false"
                    >
                      {{ getUserName() }}
                    </button>
                    <div
                      class="dropdown-menu"
                      aria-labelledby="dropdownMenuButton"
                    >
                      <a class="dropdown-item" href="#">Account Settings</a>
                      <a @click="onLogoutClicked" class="dropdown-item"
                        >Logout {{ userEmail }}</a
                      >
                    </div>
                  </div>
                </li>
                <li>
                  <ShoppingCart />
                </li>
              </ul>
            </ul>
          </div>
        </div>
      </nav>
      <div v-if="$attrs.page === 'Home'" class="row" style="margin-top: 10%">
        <div class="col-lg-10 mx-auto">
          <h1 class="text-uppercase" style="opacity: 0.7">
            <strong>Where your dream setup becomes reality.</strong>
          </h1>
          <hr />
        </div>
      </div>
      <div v-if="$attrs.page === 'Home'" class="col-lg-8 mx-auto">
        <p class="text-faded mb-5">
          We build a combination of desk and computer to improve the esthetics
          of your working environment.
        </p>
        <a class="btn btn-primary btn-xl" id="hoverButton" role="button" href="#services"
          >Find Out More</a
        >
      </div>
    </div>
  </header>
</template>


 <script>
import ShoppingCart from "./ShoppingCart.vue";
export default {
  components: { ShoppingCart },
  name: "NavHeader",
  computed: {
    userEmail() {
      return this.isLoggedIn ? this.currentUser.email : "";
    },
    isAuthenticated() {
      return this.$store.state.user.isAuthenticated;
    },
  },
  methods: {
    onLoginClicked() {
      window.location = this.$store.state.endpoints.login;
    },
    onLogoutClicked() {
      this.$store.commit("logout");
    },
    getUserName() {
      return this.$store.state.user.name;
    },
  },
};
</script>