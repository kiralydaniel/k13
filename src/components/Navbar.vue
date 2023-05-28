<template>
    <nav>
      <ul>
        <li><a href="#">Kezdőlap</a></li>
        <li><a href="#" class="scroll-link" @click.prevent="scrollToSection('.text-box-row:last-child')">Rólunk</a></li>
        <li><a href="#">Árajánlat</a></li>
        <li><a href="#">Kapcsolat</a></li>
      </ul>
    </nav>
  </template>
  
  <style src="./Style.css"></style>
  
  <script>
export default {
  name: 'AppNavbar',
  methods: {
    scrollToSection() {
      const targetElement = document.querySelector('.text-box-row:last-child');
      targetElement.scrollIntoView({ behavior: 'smooth' });
    },
  },
};
  </script>
  