<template>
  <div>
    <div class="page-header page-header-small">
      <parallax
        class="page-header-image"
        style="background-image: url('img/bg6.jpg')"
      >
      </parallax>
      <div class="content-center">
        <div class="container">
          <h1 class="title">International Resources.</h1>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title"></h2>
            <img
              v-lazy="'img/di.png'"
              style="max-width:210px"
              alt="Rounded Image"
              class="rounded"
            />

            <h5 class="description">
              According to the National Oceanic and Atmospheric Administration,
              Ted, Scambos, NSIDClead scentist, puts the potentially record low
              maximum sea ice extent tihs year down to low ice extent in the
              Pacific and a late drop in ice extent in the Barents Sea.
            </h5>
          </div>
        </div>
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title"></h2>
            <img
              v-lazy="'img/di.png'"
              style="max-width:210px"
              alt="Rounded Image"
              class="rounded"
            />

            <h5 class="description">
              According to the National Oceanic and Atmospheric Administration,
              Ted, Scambos, NSIDClead scentist, puts the potentially record low
              maximum sea ice extent tihs year down to low ice extent in the
              Pacific and a late drop in ice extent in the Barents Sea.
            </h5>
          </div>
        </div>
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title"></h2>
            <img
              v-lazy="'img/di.png'"
              style="max-width:210px"
              alt="Rounded Image"
              class="rounded"
            />

            <h5 class="description">
              According to the National Oceanic and Atmospheric Administration,
              Ted, Scambos, NSIDClead scentist, puts the potentially record low
              maximum sea ice extent tihs year down to low ice extent in the
              Pacific and a late drop in ice extent in the Barents Sea.
            </h5>
          </div>
        </div>
        <div class="separator separator-primary"></div>
      </div>
    </div>
  </div>
</template>
<script>
import { Button, FormGroupInput } from "@/components";
export default {
  name: "international",
  bodyClass: "landing-page",
  components: {
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput,
  },
  data() {
    return {
      form: {
        firstName: "",
        email: "",
        message: "",
      },
    };
  },
};
</script>
<style></style>
