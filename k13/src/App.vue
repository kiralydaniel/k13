<template>
  <div id="app">
    <AppNavbar />
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
    };
  },
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: rgb(255, 255, 255);
}

#app {
  text-align: center;
  padding: 20px;
}

header {
  margin-bottom: 20px;
}

footer {
  margin-top: 40px;
}
</style>
