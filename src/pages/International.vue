<template>
  <div>
    <div class="page-header page-header-small">
      <parallax
        class="page-header-image"
        style="background-image: url('img/bg6.jpg')"
      >
      </parallax>
      <div class="content-center">
        <img
          class="n-logo"
          style="max-height:150px"
          src="img/now-logo.png"
          alt=""
        />

        <div class="container">
          <h1 class="title">International Resources</h1>
          <div class="text-center">
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-facebook-square"></i>
            </a>
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-twitter"></i>
            </a>
            <a href="#pablo" class="btn btn-primary btn-icon btn-round">
              <i class="fab fa-google-plus"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h4 class="title">Democracy International</h4>
            <a
              class="nav-link"
              :class="{ 'btn-neutral': isHome }"
              href="https://www.democracy-international.org/"
              target="_blank"
            >
              <img
                v-lazy="'img/di.png'"
                style="max-width:210px"
                alt="Rounded Image"
                class="rounded"
              />
            </a>
            <h5 class="description">
              Democracy means that power rests with the people and not with
              kings, aristocrats, or technocrats. This is the core principle of
              democracy. Yet unfortunately, real democracy too often is not
              realised...
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
