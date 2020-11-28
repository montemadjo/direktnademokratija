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
          <h1 class="h1-seo">Izađimo iz gliba</h1>
          <h3>
            Odgajimo zdravu Crnu Goru. Srušimo barijere.
          </h3>
        </div>
        <h6 class="category category-absolute">
          Designed & coded by Mali Miško.
        </h6>
      </div>
    </div>
    <div class="main">
      <!-- <div class="section section-images">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="hero-images-container">
                <img src="img/hero-image-1.png" alt="" />
              </div>
              <div class="hero-images-container-1">
                <img src="img/hero-image-2.png" alt="" />
              </div>
              <div class="hero-images-container-2">
                <img src="img/hero-image-3.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div> -->
    </div>
    <div class="section">
      <div class="container text-center">
        <div class="row justify-content-md-center">
          <div class="col-md-12 col-lg-8">
            <h2 class="title">
              Подршка развоју Директне Демократије у Црној Гори
            </h2>
            <h5 class="description">
              Наш циљ је да укинемо страначке и све друге баријере у дијалогу.
              Да све људе који су незадовољни досадашњим стањем политчког живота
              у нашој држави, ујединимо, њихова мишљења укрупнимо, учинимо
              видљивим и тако створимо колективну снагу која ће моћи јавно да
              презентује сваки проблем поштујући захтјев општег добра. Сви
              добронамјерни људи без обзира на страначку, вјерску или било коју
              другу припадност, имаће прилику да предлажу и да учествују у
              креирању свих садржаја, којима ћемо се јавно бавити Укључите се
              активно и директно у политику!
            </h5>
          </div>
        </div>
      </div>
    </div>
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
