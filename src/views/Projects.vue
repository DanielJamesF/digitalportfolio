<template>
  <section id="projects">
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
#head {
  height: 20vh;
  display: flex;
  justify-content: center;
  align-items: center;
  border: solid #151414;
}

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
  