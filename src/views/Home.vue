<template>
    <section id="home">
        <div class="container-fluid pb-5">
            <div class="row">
                <div class="col">
                    <h1 class="h1 text p-5">Hi
                        <br>
                        <span>Daniel Fredericks</span></h1>
                    <h3 class="">Aspirings Web Developer</h3>
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
    background-image: url("https://i.postimg.cc/dttzxxJg/4230932.webp");
}

h1 {
    font-size: 60px;
    text-shadow: 2px 2px grey;
}

h3 {
    text-shadow: 2px 2px grey;
}

.text {
    font-family: "Recursive", monospace;
    font-size: clamp(4em, 15vmin, 20em);
    text-shadow: 0;
    color: black;
    animation: anime 2s cubic-bezier(0.445, 0.05, 0.55, 0.95) alternate infinite;
}

@keyframes anime {
    from {
        font-variation-settings: "wght" 800, "slnt" 0;
        text-shadow: -5px 5px 5px grey, -8px 10px 7px lightgray,
            -11px 15px 9px white;
    }

    to {
        font-variation-settings: "wght" 300, "slnt" 15;
        text-shadow: none;
    }
}
</style>