<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax
        class="page-header-image"
        style="background-image:url('img/header.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="content-center brand">
          <img class="n-logo" src="img/now-logo.png" alt="" />
          <h1 class="h1-seo">
            NVO Inicijativa Direktne Demokratije
          </h1>
          <h4>
            BUDI DIREKTAN
          </h4>
          <h2></h2>
          <a
            title="Peticija"
            data-placement="bottom"
            href="https://www.peticije.online/298227?s=79541705"
            target="_blank"
          >
            <h2>Potpiši peticiju podrške</h2>
          </a>
        </div>
        <h6 class="category category-absolute">
          Designed & coded by CDD Crna Gora.
        </h6>
      </div>
    </div>
    <div class="main"></div>
    <div class="section">
      <div class="container text-center">
        <div class="row justify-content-md-center">
          <div class="col-md-12 col-lg-8">
            <h2 class="title">
              Podrška razvoju direktne demokratije u Crnoj Gori
            </h2>
            <h5 class="description">
              Cilj nam je ukloniti stranačke i sve ostale prepreke u dijalogu.
              Ujediniti sve ljude koji su nezadovoljni trenutnim stanjem
              političkog života u našoj zemlji, proširiti njihova mišljenja,
              učiniti ih vidljivima i na taj način stvoriti kolektivnu silu koja
              će svaki problem moći javno predstaviti, poštujući zahtjev općeg
              dobra. Svi dobronamjerni ljudi, bez obzira na stranačku, vjersku
              ili bilo koju drugu pripadnost, imat će priliku predlagati i
              sudjelovati u stvaranju svih sadržaja kojima ćemo se baviti javno.
              Uključite se aktivno i direktno u politiku!
            </h5>
          </div>
        </div>
      </div>
    </div>

    <!-- <div class="section section-team text-center">
      <div class="container">
        <h2 class="title">Here is our team</h2>
        <div class="team">
          <div class="row">
            <div class="col-md-4">
              <div class="team-player">
                <img
                  src="img/avatar.jpg"
                  alt="Thumbnail Image"
                  class="rounded-circle img-fluid img-raised"
                />
                <h4 class="title">Romina Hadid</h4>
                <p class="category text-primary">Model</p>
                <p class="description">
                  You can write here details about one of your team members. You
                  can give more details about what they do. Feel free to add
                  some <a href="#">links</a> for people to be able to follow
                  them outside the site.
                </p>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-twitter"></i
                ></a>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-instagram"></i
                ></a>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-facebook-square"></i
                ></a>
              </div>
            </div>
            <div class="col-md-4">
              <div class="team-player">
                <img
                  src="img/ryan.jpg"
                  alt="Thumbnail Image"
                  class="rounded-circle img-fluid img-raised"
                />
                <h4 class="title">Ryan Tompson</h4>
                <p class="category text-primary">Designer</p>
                <p class="description">
                  You can write here details about one of your team members. You
                  can give more details about what they do. Feel free to add
                  some <a href="#">links</a> for people to be able to follow
                  them outside the site.
                </p>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-twitter"></i
                ></a>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-linkedin"></i
                ></a>
              </div>
            </div>
            <div class="col-md-4">
              <div class="team-player">
                <img
                  src="img/eva.jpg"
                  alt="Thumbnail Image"
                  class="rounded-circle img-fluid img-raised"
                />
                <h4 class="title">Eva Jenner</h4>
                <p class="category text-primary">Fashion</p>
                <p class="description">
                  You can write here details about one of your team members. You
                  can give more details about what they do. Feel free to add
                  some <a href="#">links</a> for people to be able to follow
                  them outside the site.
                </p>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-google-plus"></i
                ></a>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-youtube"></i
                ></a>
                <a href="#pablo" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-twitter"></i
                ></a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div> -->

    <signup-form></signup-form>
    <!-- <examples-section></examples-section> -->
    <!-- <download-section></download-section> -->
  </div>
</template>
<script>
import { Parallax } from "@/components";
import BasicElements from "./components/BasicElementsSection";
import Navigation from "./components/Navigation";
import TabsSection from "./components/Tabs";
import ProgressPagination from "./components/ProgressPagination";
import Notifications from "./components/Notifications";
import Typography from "./components/Typography";
import JavascriptComponents from "./components/JavascriptComponents";
import CarouselSection from "./components/CarouselSection";
import NucleoIconsSection from "./components/NucleoIconsSection";
import SignupForm from "./components/SignupForm";
import ExamplesSection from "./components/ExamplesSection";
import DownloadSection from "./components/DownloadSection";

export default {
  name: "index",
  bodyClass: "index-page",
  components: {
    Parallax,
    SignupForm,
  },
};
</script>
<style></style>
