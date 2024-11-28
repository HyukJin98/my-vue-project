<template>
    <header>
      <div class="container">
        <h1>HyukJin Lee</h1>
        <nav>
          <a href="#about">&lt; About /&gt;</a>
          <a href="#skills">&lt; Skills /&gt;</a>
          <a href="#projects">&lt; Projects /&gt;</a>
          <a href="#contact">&lt; Contact /&gt;</a>
        </nav>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: "HeaderComponent",
  };
  </script>
  
  <style scoped>
  header {
    background: #d1585800;
    color: #000000;
    padding: 20px;
  }
  nav a {
    color: #000000;
    margin: 0 10px;
    text-decoration: none;
  }
  </style>