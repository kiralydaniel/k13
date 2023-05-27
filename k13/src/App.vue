<template>
  <div id="app">
    <AppNavbar />
    <button class="scroll-button" @click="scrollToTop" v-show="showScrollButton">
      <span class="arrow-up"></span>
    </button>
    <main>
      <ChimneyUpgrade />
      <ChimneySolve />
      <p>{{ message }}</p>
    </main>
    <footer>
      <p>&copy; {{ currentYear }} K13 Mester</p>
    </footer>
  </div>
</template>

<script>
import AppNavbar from './components/Navbar.vue'
import ChimneyUpgrade from './components/ChimneyUpgrade.vue'
import ChimneySolve from './components/ChimneySolve.vue'

export default {
  components: {
    AppNavbar,
    ChimneyUpgrade,
    ChimneySolve,
  },
  data() {
    return {
      message: "Thank you for visiting!",
      currentYear: new Date().getFullYear(),
      showScrollButton: false,
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
      this.showScrollButton = scrollTop > 300;
    },
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth',
      });
    },
  },
};
</script>

