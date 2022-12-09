<template>
  <div id="testimonials" class="row">
    <h2 class="display-4">Testimonials...</h2>
    <!-- <div v-for="carouselitem in Carousel" :key="carouselitem"> -->
    <div class="col">
      <br />
      <div id="carouselIndicators" class="carousel slide border rounded-4" data-bs-ride="carousel">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="0"
            class="active rounded-pill"></button>
          <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="1" class="rounded-pill"></button>
          <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="2" class="rounded-pill"></button>
          <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="3" class="rounded-pill"></button>
          <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="4" class="rounded-pill"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="https://i.postimg.cc/3NbhYdM2/Joel.jpg" style="object-fit: cover" alt="Joel" id="image"
              class="rounded-circle" />
            <h5>{{ carouselitem.name }}</h5>
            <div id="comments">
              <p>
                {{ carouselitem.comment }}
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="https://i.postimg.cc/HpHW15CY/Clayton.jpg" style="object-fit: cover" alt="Clayton" id="image"
              class="rounded-circle" />
            <h5 class="py-3">Clayton Adonis</h5>
            <div id="comments">
              <p>
                Daniel is an absolute delight to work with and he always makes
                any room he is in better.
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="https://i.postimg.cc/cLWvzbmZ/Muddathir.jpg" style="object-fit: cover" alt="Muddathir" id="image"
              class="rounded-circle" />
            <h5>Muddathir Dawood</h5>
            <div id="comments">
              <p>
                Daniel is a developer with potential to become something great
                in the future. It is a pleasure watching his skill grow with
                each project he is given and motivates me and other to do
                better. He will add an enormous amount of value to any team
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="https://i.postimg.cc/Fspv9Cvh/Jared.jpg" style="object-fit: cover" alt="Jared" id="image"
              class="rounded-circle" />
            <h5>Jared Isaacs</h5>
            <div id="comments">
              <p>
                Daniel is an outgoing, hardworking, creative web developer.
                Who sets out to achieve his goals through perseverance and
                determination. As his colleague I see a bright future filled
                with prosperity being set in front of him, with his iron will
                to overcome any impediments that comes he way. As such he has
                the set skills to fulfill any task that will be given to him,
                making him a great asset to any business or company.
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="https://i.postimg.cc/kgSyQz5m/Reagan1.jpg" style="object-fit: cover" alt="Reagan" id="image"
              class="rounded-circle" />
            <h5>Reagan Carolussen</h5>
            <div id="comments">
              <p>
                Daniel is a trustworthy, multi-talented individual that shows
                the ability to learn and grasp new concepts quickly. He is
                focused and works will with others. I highly recommend him to
                any team or organization.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- </div> -->
  </div>
</template>
  
<script>
export default {
  computed: {
    Carousel() {
      return this.$store.state.carousel;
    },
  },
};
</script>
  
<style>
#testimonials {
  min-height: 100vh;
  padding-top: 10vh;
  padding-bottom: 10vh;
}

#image {
  aspect-ratio: 1;
  object-fit: cover;
  width: 20%;
  height: auto;
}

#comments {
  min-height: 20vh;
}
</style>