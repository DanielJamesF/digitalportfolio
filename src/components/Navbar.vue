<template>
  <nav class="fixed-top d-flex justify-content-between">
    <div class="d-flex justify-content-start bg-transparent">
      <button class="btn border-0" type="button" data-bs-toggle="offcanvas"
        data-bs-target="#offcanvasExample" aria-controls="offcanvasExample">
        <i  class="bi bi-list" style="color: lightgrey; font-size: 40px;"></i>
      </button>
    </div>
    <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
      <div class="offcanvas-header">
        <button class="btn border-0" type="button" data-bs-dismiss="offcanvas">
        <i  class="bi bi-x" style="color: lightgrey; font-size: 40px;"></i>
        </button>
      </div>
      <div class="offcanvas-body">
        <div id="navbarNav">
          <div class="navbar-nav">
            <div class="d-flex flex-column">
              <router-link @click="closebar" to="/">Home</router-link>
              <router-link @click="closebar" to="/about">About</router-link>
              <router-link @click="closebar" to="/projects">Projects</router-link>
              <router-link @click="closebar" to="/resume">Resume</router-link>
              <router-link @click="closebar" to="/testimonials">Testimonials</router-link>
              <router-link @click="closebar" to="/contact">Contact</router-link>
              <router-link @click="closebar" to="/"></router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    closebar() {
      document.getElementById("button").click();
    },
  }
};
</script>

<style scoped>
nav {
  width: 100%;
  height: 9vh;
  background: #151414;
}

nav a {
  font-weight: bold;
  color: #92989f;
  text-decoration: none;
  font-size: 40px;
  line-height: 90px;
  text-shadow: 2px 2px grey;
}

nav a:hover {
  color: white;
}
.offcanvas-header {
  height: 9vh;
  background: #151414;
}
.offcanvas-body {
  background: lightgrey;
}
</style>