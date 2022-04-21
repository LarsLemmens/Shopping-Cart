<template>
  <body
    id="page-top"
    data-bs-spy="scroll"
    data-bs-target="#mainNav"
    data-bs-offset="57"
  >
    <NavHeader :page="page" :redirect="redirect" />
    <section id="about" class="bg-primary" style="padding: 1rem">
      <div class="container">
        <div class="row">
          <div class="col offset-lg-8 text-center mx-auto">
            <h2 class="text-white section-heading">Desks</h2>
            <hr class="light my-4" />
            <p class="text-faded mb-4">
              Here is an overview of all the pre-build desks we currently have
              available.&nbsp;
            </p>
          </div>
        </div>
      </div>
    </section>

    <div>
      <div class="projects-clean">
        <div class="row projects">
          <Item v-for="product in products" :key="product.id" :item="product" />
        </div>
        <a class="btn btn-primary btn-xl" role="button" href="#services"
          >See more!</a
        >
      </div>
    </div>
  </body>
</template>

<script>
import NavHeader from "@/NavHeader.vue";
import Item from "@/Item.vue";
export default {
  computed: {
    products() {
      return this.$store.state.products;
    },
    isAuthenticated() {
      return this.$store.state.user.isAuthenticated;
    },
  },
  components: {
    NavHeader,
    Item,
  },
  data() {
    return {
      page: "Builder",
      redirect: "Home",
    };
  },
};
</script>


<style>
@import "https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800";
@import "https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800";
@import "https://fonts.googleapis.com/css?family=Merriweather:400,300,300italic,400italic,700,700italic,900,900italic";
@import "https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css";

@import "https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/17.0.8/css/intlTelInput.css";
@import "https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/17.0.8/js/intlTelInput.min.js";
@import "https://www.google.com/recaptcha/api.js";
</style>


<style scoped>
@import "../assets/css/Projects-Clean.css";
@import "../assets/css/Features-Boxed.css";
</style>
