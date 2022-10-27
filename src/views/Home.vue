<template>
    <section id="home">
        <div class="container-fluid pb-5">
            <div class="row">
                <div class="col">
                    <h3>Aspirings Web Developer</h3>
                    <h1 class="h1">Hi I am <span>Daniel Fredericks</span></h1>
                </div>
            </div>
        </div>
    </section>
</template>
  
<script>
export default {
    components: {},
};
</script>
  
<style scoped>

#home {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background-size: cover;
    background-position: center;
    position: relative;
    background: url('http://unsplash.it/1200x800') center center no-repeat;
    background-size: cover;
    background-image: linear-gradient(to bottom right, white, black);
}


h1 {
    font-size: 60px;
    text-shadow: 2px 2px grey;
}

h3 {
    text-shadow: 2px 2px grey;
}
</style>