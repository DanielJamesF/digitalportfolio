<template>
    <section id="home">
        <div class="container-fluid pb-5">
            <div class="row">
                <div class="col">
                    <h3>Aspirings Web Developer</h3>
                    <h1 class="h1">Hi I am Daniel Fredericks</h1>
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
    background-image: url("https://i.postimg.cc/PJsnNmLz/mountain.webp");
    background-size: cover;
    background-position: center;
    color: white;
    border-bottom: solid 1px white;
}

h1 {
    font-size: 60px;
    text-shadow: 2px 2px grey;
}

h3 {
    text-shadow: 2px 2px grey;
}
</style>