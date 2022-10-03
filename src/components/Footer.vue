<template>
    <footer>
        <div class="container-fluid">

            <div class="row">
                <div class="col">
                    <h3>Quick links: </h3>
                    <ul class="list-unstyled">
                        <li class="pb-1">
                            <router-link to="/"></router-link>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h3>Reach out: </h3>
                    <ul class="list-unstyled">
                        <li class="pb-1">
                            <a class="text-decoration-none pb-1" href="https://app.netlify.com/teams/danieljamesf/overview">
                                <i class=""></i> Netlify</a>
                        </li>
                        <li class="pb-1">
                            <a class="text-decoration-none" href="https://github.com/DanielJamesF">
                                <i class="bi bi-github"></i> Github</a>
                        </li>
                        <li class="pb-1">
                            <a class="text-decoration-none"
                                href="https://www.linkedin.com/in/daniel-fredericks-85744023a/"><i
                                    class="bi bi-linkedin"></i> Linkedin</a>
                        </li>
                        <li>
                            <a class="text-decoration-none" href="mailto:fredericksd17@gmail.com">
                                <i class="bi bi-envelope"> Email</i>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <br />
        </div>
        <v-footer v-bind="localAttrs">
            &copy; Copyright {{ new Date().getFullYear() }}
        </v-footer>
    </footer>
</template>
  
<script>
export default {
    name: "Footer",
};
</script>
<style>
footer {
    background-color: black;
    color: white;
}

a {
    color: white;
}

a:hover {
    color: grey;
}
</style>