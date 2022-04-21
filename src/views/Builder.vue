<template>
  <body
    id="page-top"
    data-bs-spy="scroll"
    data-bs-target="#mainNav"
    data-bs-offset="57"
  >
    <NavHeader :page="page" :redirect="redirect" />
    <section id="about" class="bg-primary">
      <div class="container">
        <div class="row">
          <div class="col offset-lg-8 text-center mx-auto">
            <h2 class="text-white section-heading">Desks</h2>
            <hr class="light my-4" />
            <p class="text-faded mb-4">
              This is an overview of all the pre-build desks.&nbsp;
            </p>
            <a
              class="btn btn-light btn-xl"
              role="button"
              href="#services"
              data-toggle="modal"
              data-target="#exampleModalCenter"
              >See more!</a
            >
          </div>
        </div>
      </div>
    </section>

    <!-- Modal -->
    <div
      class="modal fade"
      id="exampleModalCenter"
      tabindex="-1"
      role="dialog"
      aria-labelledby="exampleModalCenterTitle"
      aria-hidden="true"
      v-if="!isAuthenticated"
    >
      <div class="modal-dialog modal-dialog-centered" role="document">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLongTitle">
              Not logged in
            </h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true">&times;</span>
            </button>
          </div>
          <div class="modal-body">
            You have to be logged in to be able to see the pre-build desks.
          </div>
          <div class="modal-footer">
            <button type="button" class="btn btn-primary" data-dismiss="modal">
              Close
            </button>
          </div>

          <!-- Modal -->
          <div
            class="modal fade"
            id="exampleModalCenter"
            tabindex="-1"
            role="dialog"
            aria-labelledby="exampleModalCenterTitle"
            aria-hidden="true"
            v-if="isAuthenticated"
          >
            <div class="modal-dialog modal-dialog-centered" role="document">
              <div class="modal-content">
                <div class="modal-header">
                  <h5 class="modal-title" id="exampleModalLongTitle">
                    Name of desk
                  </h5>
                  <button
                    type="button"
                    class="close"
                    data-dismiss="modal"
                    aria-label="Close"
                  >
                    <span aria-hidden="true">&times;</span>
                  </button>
                </div>
                <div class="modal-body">
                  These are the specifications of this desk with name ...
                </div>
                <div class="modal-footer">
                  <button
                    type="button"
                    class="btn btn-primary"
                    data-dismiss="modal"
                  >
                    Close
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="row projects">
          <Item v-for="product in products" :key="product.id" :item="product" />
        </div>
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
