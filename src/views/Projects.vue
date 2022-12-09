<template>
  <section id="projects">
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
  display: flex;
  justify-content: center;
  flex-direction: column;

}

h2 {
  font-size: 70px;
  text-shadow: 2px 2px grey;
}
</style>
  