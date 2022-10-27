<template>
    <section id="projects" class="flex-column bg-dark d-flex align-items-center">
      <h2>Projects</h2>
      <div class="container-fluid row">
        <Card />
      </div>
    </section>
  </template>
  
  <script>
  import Card from "../components/Card.vue";
  export default {
    components: { Card },
  };
  </script>
  
  <style scoped>
  #projects {
    min-height: 100vh;
    padding: 80px;
  }
  h2{
    text-shadow: 2px 2px white;
  }
  </style>
  