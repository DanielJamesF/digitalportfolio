<template>
  <section id="about">
    <div class="container-fluid p-5">
      <h2>About me</h2>
      <div class="row shadow">
        <div class="col">
          <div style="object-fit: cover; height: 200px; aspect-ratio: 1; position: relative; border-radius: 50%; overflow: hidden;" class="mx-auto">
            <img
              id="image"
              class="img-fluid"
              style="position: absolute; top: 0; left: 0;"
              src="https://i.postimg.cc/90BpLycC/about-Image.png"
              alt="daniel"
            />
          </div>
          <div>
            <h3>Bio</h3>
            <div>
              <p>
                My name is Daniel Fredericks I was born on the 7th of January
                2002 and am currently am 20 years old. I am a student at life
                Choices Academy where I am studying coding in order to become a
                Web Developer in the future. My passsion for coding stems from
                my love of technology and anything related to it. I am a hard
                worker and am able to work well in groups as I believe that I am
                able to get along with people pretty well.
              </p>
            </div>
            <h3>Hobbies</h3>
            <div>
              <p>
                I enjoy playing soccer, whether it's eleven a side or five a
                side, listening to music, mostly rap however I do enjoy listing
                to other genres as well, reading manga, watching anime, and
                going out with friends, I esecially enjoy spending time with
                those that I am close with.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#about {
  min-height: 100vh;
  padding: 80px;
}
h2 {
  font-size: 70px;
  text-shadow: 2px 2px grey;
}
h3{
  text-shadow: 2px 2px grey;
}
</style>
