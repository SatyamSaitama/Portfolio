<template>
  <div>
    <header id="header" class="d-flex flex-column justify-content-center">
      <nav id="navbar" class="navbar nav-menu">
        <ul>
          <li>
  <a href="#mode" class="nav-link scrollto active" @click="toggleMode">
    <i :class="`bx bx-${mode}`"></i> <span>Switch</span>
  </a>
</li>
          <li><a href="#hero" class="nav-link scrollto active"><i class="bx bx-home"></i> <span>Home</span></a></li>
          <li><a href="#about" class="nav-link scrollto"><i class="bx bx-user"></i> <span>About</span></a></li>
          <li><a href="#resume" class="nav-link scrollto"><i class="bx bx-file-blank"></i> <span>Resume</span></a></li>
          <li><a href="#portfolio" class="nav-link scrollto"><i class="bx bx-book-content"></i> <span>Portfolio</span></a></li>
          <li><a href="#contact" class="nav-link scrollto"><i class="bx bx-envelope"></i> <span>Contact</span></a></li>
        </ul>
      </nav><!-- .nav-menu -->
    </header><!-- End Header -->

    <!-- Hero Section -->
    <section id="hero" class="d-flex flex-column justify-content-center">
      <div class="container" data-aos="zoom-in" data-aos-delay="100">
        <h1>Satyam Kumar</h1>
        <p>I'm <span class="typed" data-typed-items=" Web Developer, ML Engineer, Web designer"></span></p>
        <div class="social-links">
          <a href="#" class="instagram"><i class="bx bxl-instagram"></i></a>
          <a href="#" class="google-plus"><i class="bx bxl-github"></i></a>
          <a href="#" class="linkedin"><i class="bx bxl-linkedin"></i></a>
        </div>
      </div>
    </section><!-- End Hero -->
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      mode: 'sun',
    };
  },
  methods: {
    toggleMode() {
      this.mode = this.mode === 'sun' ? 'moon' : 'sun';
    },
  },
};
</script>

<style scoped>
/* Add your component-specific styles here */
</style>
