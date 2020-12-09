<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link v-popover:popover1 class="navbar-brand" to="/">
        <img
          class="n-logo"
          src="img/now-logo-full.png"
          style="max-height:25px"
          alt=""
        />
        CDD Crna Gora
      </router-link>
      <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">
          Zajedno možemo mnogo. Pogledaj kako da nam se pridružiš.
        </div>
      </el-popover>
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Home</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>International resources</p>
        </a>
        <el-popover
          ref="popover2"
          popper-class="popover"
          placement="bottom"
          width="200"
          trigger="hover"
        >
          <div class="popover-body">
            Dio smo međunarodnog tima.
          </div>
        </el-popover>
      </li>
      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>O nama</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          v-popover:popover5
          class="nav-link btn btn-neutral"
          href="https://www.direktnademokratija.me/manifest"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Statut</p>
        </a>
        <el-popover
          ref="popover5"
          popper-class="popover"
          placement="bottom"
          width="200"
          trigger="hover"
        >
          <div class="popover-body">
            Download-ujte i pročitajte naš Statut.
          </div>
        </el-popover>
      </li>
      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Lokalni projekti</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Globalni projekat</p>
        </a>
      </li>

      <li class="nav-item">
        <a
          v-popover:popover2
          class="nav-link"
          href="https://www.direktnademokratija.me"
          target="_blank"
        >
          <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
          <p>Sugestije</p>
        </a>
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
};
</script>

<style scoped></style>
