<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.direktnademokratija.me">
              Kontakt
            </a>
          </li>
          <li>
            <a href="https://www.direktnademokratija.me">
              O Nama
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">&copy; {{ year }}, Designed by IDD Crna Gora.</div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String,
  },
  data() {
    return {
      year: new Date().getFullYear(),
    };
  },
};
</script>
<style></style>
