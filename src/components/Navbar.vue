<template>
  <nav class="fixed-top">
    <div class="d-flex justify-content-start bg-transparent">
      <button
        id="button"
        class="btn border-0"
        type="button"
        data-bs-toggle="offcanvas"
        data-bs-target="#offcanvasExample"
        aria-controls="offcanvasExample"
      >
        <i class="bi bi-arrow-bar-right" style="color: black; font-size: 50px;"></i>
      </button>
    </div>
    <div
      class="offcanvas offcanvas-start"
      tabindex="-1"
      id="offcanvasExample"
      aria-labelledby="offcanvasExampleLabel"
    >
      <div class="offcanvas-header">
        <button
          type="button"
          class="btn-close"
          data-bs-dismiss="offcanvas"
          aria-label="Close"
        ></button>
      </div>
      <div class="offcanvas-body">
        <div id="navbarNav">
          <div class="navbar-nav">
            <div class="d-flex flex-column">
              <router-link @click="closebar" to="/"
                >Home</router-link
              >
              <router-link @click="closebar" to="/about"
                >About</router-link
              >
              <router-link @click="closebar" to="/projects"
                >Projects</router-link
              >
              <router-link @click="closebar" to="/resume"
                >Resume</router-link
              >
              <router-link @click="closebar" to="/testimonials"
                >Testimonials</router-link
              >
              <router-link @click="clossebar" to="/contact">Contact</router-link>
              <router-link @click="closebar" to="/"
                ></router-link
              >
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

<style>
nav {
  width: 100%;
  height: 10vh;
}

nav a {
  font-weight: bold;
  color: #92989f;
  text-decoration: none;
  font-size: 40px;
  line-height: 90px;
  text-shadow: 2px 2px grey;
}

nav a:hover{
  color: white;
}

nav a.router-link-exact-active {
  color: black;
}
</style>