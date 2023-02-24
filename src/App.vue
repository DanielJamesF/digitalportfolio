<template>
  <Navbar />
  <router-view />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Navbar,
    Footer
  },
};
</script>

<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css");
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  font-size: calc(1px + 1vw);
  line-height: calc(1.1em + 0.5vw);
}
* {
  font-family: "Trirong", serif;
}

#section {
  min-height: 100vh;
  padding: 80px;
  display: flex;
  flex-direction: column;
}

#head {
  height: 20vh;
  display: flex;
  justify-content: center;
  align-items: center;
  /* border: solid #151414; */
}

h2 {
  font-size: 70px;
  text-shadow: 3px 3px 3px gray;
  border-bottom: solid black 1px;
}

h3 {
  font-size: 50px;
  color: darkgrey;
  text-shadow: 2px 2px 2px rgb(0, 0, 0);
}

h4 {
  font-size: 30px;
  text-shadow: 1px 1px 1px gray;
}

</style>
