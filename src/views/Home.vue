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
    <section id="services">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading">At Your Service</h2>
            <hr class="my-4" />
          </div>
        </div>
      </div>
      <div class="container">
        <div class="row">
          <div class="col-md-6 col-lg-3 text-center">
            <div class="mx-auto service-box mt-5">
              <i class="fa fa-solid fa-desktop"></i>
              <h3 class="mb-3">Desks</h3>
              <p class="text-muted mb-0">
                High quality desks with components of your choice.
              </p>
            </div>
          </div>
          <div class="col-md-6 col-lg-3 text-center">
            <div class="mx-auto service-box mt-5">
              <i class="fa fa-solid fa-gear"></i>
              <h3 class="mb-3">Components</h3>
              <p class="text-muted mb-0">
                Buy seperate components for your computer.
              </p>
            </div>
          </div>
          <div class="col-md-6 col-lg-3 text-center">
            <div class="mx-auto service-box mt-5">
              <i class="fa fa-solid fa-calendar"></i>
              <h3 class="mb-3">Up to Date</h3>
              <p class="text-muted mb-0">We keep up with the latest</p>
              <p class="text-muted mb-0">software and hardware.&nbsp;</p>
            </div>
          </div>
          <div class="col-md-6 col-lg-3 text-center">
            <div class="mx-auto service-box mt-5">
              <i class="fa fa-solid fa-heart"></i>
              <h3 class="mb-3">Made with Love</h3>
              <p class="text-muted mb-0">You have to love your desk again.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="text-white bg-dark">
      <div class="container text-center">
        <h2 class="mb-4">Our catalog&nbsp;</h2>
        <a
          class="btn btn-light btn-xl sr-button"
          role="button"
          data-aos="zoom-in"
          data-aos-duration="400"
          data-aos-once="true"
          href="#"
          >Download Now!</a
        >
      </div>

      <section id="portfolio" class="p-0">
        <div class="container-fluid p-0">
          <div class="row g-0 popup-gallery">
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk4.png"
                ><img class="img-fluid" src="../assets/img/desk4.png" />
                <div class="portfolio-box-caption">
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Hanging Desk</span>
                    </div>
                    <div class="project-name">
                      <span>Ideal for home office.</span>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk2.png"
                ><img class="img-fluid" src="../assets/img/desk2.png" />
                <div class="portfolio-box-caption">
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Desk type red</span>
                    </div>
                    <div class="project-name">
                      <span>Let your inner flame work.</span>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk3.png"
                ><img class="img-fluid" src="../assets/img/desk3.png" />
                <div class="portfolio-box-caption">
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Desk type green</span>
                    </div>
                    <div class="project-name">
                      <span>Let de green relax your mind.</span>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk1.png"
                ><img class="img-fluid" src="../assets/img/desk1.png" />
                <div
                  class="portfolio-box-caption"
                  style="/*background-image: white;*/"
                >
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Industrial red</span>
                    </div>
                    <div class="project-name">
                      <span>Intensive red body.</span>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk5.png"
                ><img class="img-fluid" src="../assets/img/desk5.png" />
                <div class="portfolio-box-caption">
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Desk</span>
                    </div>
                    <div class="project-name">
                      <span
                        >Working area before there is an computer in it.</span
                      >
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-6 col-lg-4">
              <a class="portfolio-box" href="../assets/img/desk6.png"
                ><img class="img-fluid" src="../assets/img/desk6.png" />
                <div class="portfolio-box-caption">
                  <div class="portfolio-box-caption-content">
                    <div class="project-category text-faded">
                      <span>Calm</span>
                    </div>
                    <div class="project-name">
                      <span>No lights added, just focus and clean.</span>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
        </div>
      </section>
    </section>
    <section id="contact">
      <div class="container">
        <div class="row">
          <div class="col-lg-8 text-center mx-auto">
            <h2 class="section-heading">Let's Get In Touch!</h2>
            <hr class="my-4" />
            <p class="mb-5">
              <br />Ready for your first build-in-desk computer of do you need
              more information?<br />Do not hesitate to contact us!
            </p>
          </div>
          <form class="formform">
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input
                type="email"
                class="form-control"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
                placeholder="Enter email"
              />
              <small id="emailHelp" class="form-text text-muted"
                >We'll never share your email with anyone else.</small
              >
            </div>
            <div class="form-group">
              <label for="exampleTelephoneNumber1">Telephone number</label>
              <input
                type="tel"
                class="form-control"
                id="exampleTelephoneNumber1"
                placeholder="Enter telephone number"
              />
            </div>
            <div
              class="g-recaptcha brochure__form__captcha"
              data-sitekey="6Lenz4YfAAAAAIAdnIjvI_kkU9O1uH3gSeYjvPSG"
            ></div>
            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>
        <div class="row">
          <div class="col-lg-4 text-center ms-auto">
            <i
              class="fa fa-phone fa-3x mb-3 sr-contact"
              data-aos="zoom-in"
              data-aos-duration="300"
              data-aos-once="true"
            ></i>
            <p>+32-496-248-189</p>
          </div>
          <div class="col-lg-4 text-center me-auto">
            <i
              class="fa fa-envelope-o fa-3x mb-3 sr-contact"
              data-aos="zoom-in"
              data-aos-duration="300"
              data-aos-delay="300"
              data-aos-once="true"
            ></i>
            <p>
              <a href="mailto:your-email@your-domain.com">info@dreamdesk.be</a>
            </p>
          </div>
        </div>
      </div>
    </section>
  </body>
</template>

<script>
import NavHeader from "@/NavHeader.vue";
export default {
  components: {
    NavHeader,
  },
  data() {
    return {
      page: "Home",
      redirect: "",
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