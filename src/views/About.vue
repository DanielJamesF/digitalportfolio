<template>
  <section id="about">
    <div class="row" id="head">
      <div class="col">
        <h2>About me</h2>
      </div>
    </div>
    <div class="row">
      <div class="col-md"></div>
      <div class="col-md-4">
        <div>
          <img id="image" class="img-fluid"
            src="https://i.postimg.cc/76HfWqdz/about-Image-Photo-Room-removebg-preview.png" alt="daniel" />
        </div>
      </div>
      <div class="col-md-6" id="about-bio">
        <h3>Bio</h3>
        <p>
          My name is Daniel Fredericks I was born on the 7th of January
          2002. I attended a six month coding bootcamp at life
          Choices Coding Academy in order to persue my aspirations of becoming a
          Web Developer. My passsion for coding stems from
          my love of technology which has always been an interest of mine since I was really young. I am a hard
          worker and am able to work well in groups as I believe that I am
          able to get along with people pretty well.
        </p>
        <h3>Hobbies</h3>
        <p>
          My hobbies include watching coding videos on YouTube and looking at codes on CodePen to improve on my
          creativity and to broaden my view on different ways code can be used and implemented. I also enjoy sports
          and watching anime as an escape and stress reliever from the work environment.
        </p>
      </div>
      <div class="col-md"></div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#head {
  height: 20vh;
  display: flex;
  justify-content: center;
  align-items: center;
  border: solid #151414;
}

#about {
  min-height: 100vh;
  padding: 80px;
  display: flex;
  flex-direction: column;
}

h2 {
  font-size: 70px;
  text-shadow: 2px 2px gray;
}

h3 {
  text-shadow: 2px 2px gray;
}

.img-fluid{
  object-fit: cover;
}

#about-bio{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media(min-width: 375px) {
  .mx-auto {
    height: 200px;
  }
}
</style>
