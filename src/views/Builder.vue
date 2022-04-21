<template>
  <body
    id="page-top"
    data-bs-spy="scroll"
    data-bs-target="#mainNav"
    data-bs-offset="57"
  >
    <NavHeader :page="page" />
    <h1>Builder</h1>
    <section id="about" class="bg-primary">
      <div class="container">
        <div class="row">
          <div class="col offset-lg-8 text-center mx-auto">
            <h2 class="text-white section-heading">
              A messy desk is a messy head!
            </h2>
            <hr class="light my-4" />
            <p class="text-faded mb-4">
              This is what we improve to your setup. Built-in-desk computers are
              what will make you more productive.<br />Companies like Mircrosoft
              and Acer already showed their interesse.&nbsp;
            </p>
            <a class="btn btn-light btn-xl" role="button" href="#services"
              >Get Started!</a
            >
          </div>
        </div>
      </div>
    </section>

    <div>
      <h1>Builder</h1>

      <div class="projects-clean">
        <div class="container">
          <div class="intro">
            <h2 class="text-center">Desks</h2>
            <p class="text-center">
              This is an overview of all the pre-build desks.
            </p>
          </div>
          <div class="row projects">
            <Item
              v-for="product in products"
              :key="product.id"
              :item="product"
            />
          </div>
        </div>
      </div>
    </div>
  </body>
</template>

<!--
          <div class="col-sm-6 col-lg-4 item">
            <img class="img-fluid" src="assets/img/desk.jpg" />
            <h3 class="name">Hanging desk</h3>
            <p class="description">A desk that has to be mounted to the wall</p>
          </div>
          <div class="col-sm-6 col-lg-4 item">
            <img class="img-fluid" src="assets/img/building.jpg" />
            <h3 class="name">Red desk</h3>
            <p class="description">
              A desk that has a color scheme that exists out of black and red
            </p>
          </div>
          <div class="col-sm-6 col-lg-4 item">
            <img class="img-fluid" src="assets/img/building.jpg" />
            <h3 class="name">Green desk</h3>
            <p class="description">
              <br />A desk that has a color scheme that exists out of black and
              green<br />
            </p>
          </div>
          <div class="col-sm-6 col-lg-4 item">
            <img class="img-fluid" src="assets/img/building.jpg" />
            <h3 class="name">Zen desk</h3>
            <p class="description">
              <br />A desk that has almost no lights, this one is very clean and
              steady<br /><br />
            </p>
          </div>
          <div class="col-sm-6 col-lg-4 item">
            <img class="img-fluid" src="assets/img/building.jpg" />
            <h3 class="name">Industrial red desk</h3>
            <p class="description">
              <br />A desk that has a color scheme that exists out of black and
              industrial red<br />
            </p>
          </div>
-->

<!--    
<script>
// @ is an alias to /src
import Item from "@/Item.vue";
export default {
  name: "Home",
  computed: {
    products() {
      return this.$store.state.products;
    },
  },
  components: {
    Item,
  },
};
</script>
-->
<script>
import NavHeader from "@/NavHeader.vue";
import Item from "@/Item.vue";
export default {
  name: "Home",
  computed: {
    products() {
      return this.$state.products;
    },
  },
  components: {
    NavHeader,
    Item,
  },
  data() {
    return {
      page: "Builder",
    };
  },
};
</script>


<style>
@import "../assets/css/bootstrap.min.css";

@import "https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800";
@import "https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800";
@import "https://fonts.googleapis.com/css?family=Merriweather:400,300,300italic,400italic,700,700italic,900,900italic";
@import "https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css";

@import "https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/17.0.8/css/intlTelInput.css";
@import "https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/17.0.8/js/intlTelInput.min.js";
@import "https://www.google.com/recaptcha/api.js";
</style>


<style scoped>
@import "../assets/css/bootstrap.min.builder.css";
@import "../assets/css/Projects-Clean.css";
@import "../assets/css/Features-Boxed.css";
</style>
