<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link class="navbar-brand" to="/">
        <img
          class="n-logo"
          src="img/now-logo-full.png"
          style="max-height: 25px"
          alt=""
        />
        IDD Crna Gora
      </router-link>
    </template>
    <template slot="navbar-menu">
      <li class="nav-item" @click="homeClicked">
        <router-link class="nav-link" :class="{ 'btn-neutral': isHome }" to="/">
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Home</p>
        </router-link>
      </li>
      <li class="nav-item" @click="internationalClicked">
        <router-link
          class="nav-link"
          :class="{ 'btn-neutral': isInternational }"
          to="/international"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>International resources</p>
        </router-link>
      </li>
      <!-- <li class="nav-item" @click="aboutClicked">
        <router-link
          class="nav-link"
          :class="{ 'btn-neutral': isAbout }"
          to="/about"
        >
          <p>O nama</p>
        </router-link>
      </li> -->
      <li class="nav-item" @click="statutClicked">
        <a
          class="nav-link"
          :class="{ 'btn-neutral': isStatut }"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Statut</p>
        </a>
      </li>
      <li class="nav-item" @click="localClicked">
        <router-link
          v-popover:popover2
          :class="{ 'btn-neutral': isLocal }"
          class="nav-link"
          to="/local"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Lokalni projekti</p>
        </router-link>
      </li>
      <li class="nav-item" @click="globalClicked">
        <router-link
          v-popover:popover2
          class="nav-link"
          :class="{ 'btn-neutral': isGlobal }"
          to="/global"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Globalni projekat</p>
        </router-link>
      </li>
      <li class="nav-item" @click="suggestionsClicked">
        <router-link
          v-popover:popover2
          class="nav-link"
          :class="{ 'btn-neutral': isSuggestions }"
          to="/sugestions"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Sugestije</p>
        </router-link>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Follow us on Twitter"
          data-placement="bottom"
          href="https://twitter.com/direktnademokratijame"
          target="_blank"
        >
          <i class="fab fa-twitter"></i>
          <p class="d-lg-none d-xl-none">Twitter</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Like us on Facebook"
          data-placement="bottom"
          href="https://www.facebook.com/direktnademokratijame"
          target="_blank"
        >
          <i class="fab fa-facebook-square"></i>
          <p class="d-lg-none d-xl-none">Facebook</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Follow us on Instagram"
          data-placement="bottom"
          href="https://www.instagram.com/direktnademokratijame"
          target="_blank"
        >
          <i class="fab fa-instagram"></i>
          <p class="d-lg-none d-xl-none">Instagram</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { Navbar } from "@/components";
import { Popover } from "element-ui";

const STATUS_HOME = 0,
  STATUS_INTERNATIONAL = 1,
  STATUS_ABOUT = 2,
  STATUS_LOCAL = 3,
  STATUS_GLOBAL = 4,
  STATUS_SUGGESTIONS = 5,
  STATUS_STATUT = 6;

export default {
  name: "main-navbar",
  props: {
    transparent: Boolean,
    colorOnScroll: Number,
  },
  components: {
    Navbar,

    [Popover.name]: Popover,
  },
  data() {
    return {
      currentStatus: 0,
    };
  },
  computed: {
    isHome() {
      return this.currentStatus === STATUS_HOME;
    },
    isInternational() {
      return this.currentStatus === STATUS_INTERNATIONAL;
    },
    isAbout() {
      return this.currentStatus === STATUS_ABOUT;
    },
    isStatut() {
      return this.currentStatus === STATUS_STATUT;
    },
    isLocal() {
      return this.currentStatus === STATUS_LOCAL;
    },
    isGlobal() {
      return this.currentStatus === STATUS_GLOBAL;
    },
    isSuggestions() {
      return this.currentStatus === STATUS_SUGGESTIONS;
    },
  },
  methods: {
    homeClicked() {
      this.currentStatus = STATUS_HOME;
    },
    internationalClicked() {
      this.currentStatus = STATUS_INTERNATIONAL;
    },
    aboutClicked() {
      this.currentStatus = STATUS_ABOUT;
    },
    statutClicked() {
      this.currentStatus = STATUS_STATUT;
    },
    localClicked() {
      this.currentStatus = STATUS_LOCAL;
    },
    globalClicked() {
      this.currentStatus = STATUS_GLOBAL;
    },
    suggestionsClicked() {
      this.currentStatus = STATUS_SUGGESTIONS;
    },
  },
};
</script>

<style scoped></style>
