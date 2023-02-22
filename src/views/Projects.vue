<template>
  <section id="section">
    <div class="row" id="head">
      <div class="col">
        <h2>Projects</h2>
      </div>
    </div>
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
h2 {
  font-size: 70px;
  text-shadow: 2px 2px grey;
}
</style>