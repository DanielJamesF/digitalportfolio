<template>
  <div v-for="project in Projects" :key="project" class="col-md-3 border-0">
    <div class="card d-flex align-items-center justify-content-center border-0">
      <div class="container d-flex align-items-center justify-content-center rounded-0 shadow">
        <img :src="project.image" :alt="project.title" />
        <div class="meta">
          <h2>{{ project.title }}</h2>
          <p>
            {{ project.desc }}
          </p>
          <div class="row">
            <div class="col px-1">
              <button type="button">
                <a v-bind:href="project.live" target="_blank">Live</a>
              </button>
            </div>
            <div class="col px-1">
              <button type="button">
                <a v-bind:href="project.github" target="_blank">Github</a>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
  
<script>
export default {
  computed: {
    Projects() {
      return this.$store.state.projects;
    },
  },
};
</script>
  
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800;900&display=swap");

/*
  ===========================================================
    ROOT 
  ===========================================================
   */

:root {
  --clr-primary: hsl(5, 86%, 44%);
  --body-bg: linear-gradient(120deg, hsl(0, 0%, 18%) 10%, hsl(0, 0%, 2%));
  --inner-bg: black;

  --card-inner-width: 14em;
  --card-inner-height: 21em;

  /* animation props */
  --ty-duration: 0.6s;
  --bar-grow-duration: 0.4s;
  --visible-duration: 0.4s;
  --visible-delay: 0.6s;
  --bg-zoom-duration: 0.4s;
}

/*
  ===========================================================
    RESET 
  ===========================================================
   */
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}


@media (prefers-reduced-motion: reduce) {

  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}

/* ----- */

body {
  background: var(--body-bg);
  display: flex;
  align-items: center;
  justify-content: center;

  font-family: "Montserrat";
  line-height: 1.2rem;
}

/*
  ===========================================================
    DEFINTIONS 
  ===========================================================
   */
.card {
  background: var(--card-bg, none);
  color: var(--card-default-color, white);
  padding: var(--card-padding, 1rem);
}

/* container */
.card>.container {
  width: var(--card-inner-width, 14em);
  height: var(--card-inner-height, 21em);

  position: relative;
  overflow: hidden;

  background: var(--inner-bg, grey);
  background-size: cover;

  border-radius: var(--inner-border-radius, 1em);
}

/* image */
.card>.container>img {
  width: 100%;
  object-fit: cover;

  /* valid for non-pointer devices also */
  transition-duration: var(--bg-zoom-duration, 1s);
  transition-property: transform;
}

/* meta group */
.card>.container>.meta {
  position: absolute;
  padding: var(--inner-padding, 1rem);
  bottom: 0;
  width: 100%;

  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
  gap: 0.8rem;

  background: linear-gradient(hsla(0, 0%, 0%, 0),
      hsla(0, 0%, 0%, 0.6) 10%,
      hsla(0, 0%, 0%, 1));
}

/*    title */
.card>.container>.meta>h2 {
  font-weight: 500;
  font-size: 1.2rem;
  line-height: 1.8rem;
  position: relative;
  max-width: 100%;
  width: max-content;
}

/* decorative line below the title*/
.card>.container>.meta>h2::after {
  content: "";
  position: absolute;
  width: calc(100% + var(--inner-padding, 1rem));
  height: 3px;
  left: calc(var(--inner-padding, 1rem) * -1);
  bottom: 0;
  background-color: var(--clr-primary, hsl(0, 50%, 50%));
}

/*    paragraph */
.card>.container>.meta>p {
  font-size: 0.8rem;
  letter-spacing: 0.015em;
}

/*    card button*/
.card>.container>.meta>.row>.col>button {
  all: unset;
  background-color: var(--clr-primary, hsl(0, 50%, 50%));
  color: var(--card-default-color, white);
  padding: 0.4rem;
  border-radius: 0.4rem;
  cursor: pointer;
  text-transform: capitalize;
  font-size: 0.7rem;
  font-weight: 600;
  letter-spacing: 0.015em;
}

/*
  ===========================================================
   HOVER, FOCUS-WITHIN EFFECT 
  ===========================================================
   */

@media (hover) {
  .card>.container>.meta {
    transform: translateY(74%);

    transition-property: transform;
    transition-duration: var(--ty-duration, 0.4s);
    transition-timing-function: ease;
  }

  .card>.container>.meta>h2::after {
    transform-origin: left;
    transform: scaleX(0);
  }

  .card>.container>.meta>*:not(h2) {
    opacity: 0;
    transform: translateY(20%);

    transition-duration: var(--visible-duration, 0.4s);
    transition-property: transform, opacity;
    transition-timing-function: linear;
  }
}

/*
    hover and focus-within state 
  */
.card:where(:hover, :focus-within)>.container>img {
  transform: scale(1.2);
  transition-timing-function: ease-in;
}

.card:where(:hover, :focus-within)>.container>.meta {
  transform: translateY(0);
  transition-delay: var(--bar-grow-duration, 1s);
}

.card:where(:hover, :focus-within)>.container>.meta>h2::after {
  transform: scaleX(1);

  transition-duration: var(--bar-grow-duration, 0.4s);
  transition-property: transform;
  transition-timing-function: ease;
}

.card:is(:hover, :focus-within)>.container>.meta>* {
  opacity: 1;
  transform: translateY(0);
  transition-delay: var(--visible-delay, 0.4s);
}

/*
    Resolving bad behaviour on tab key press
   */
.card:focus-within>.container>img {
  transition-duration: 0s;
}

.card:focus-within>.container>.meta {
  transition-duration: 0s;
  transition-delay: 0s;
}

.card:focus-within>.container>.meta>h2::after {
  transition-duration: 0s;
  transition-delay: 0s;
}

.card:focus-within>.container>.meta>* {
  transition-duration: 0s;
  transition-delay: 0s;
}
</style>