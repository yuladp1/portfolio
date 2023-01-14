<template>
  <div class="wrapper" id="particles-js">
    <AboutMe />
    <SandboxProjects />
  </div>
</template>

<script>
import AboutMe from "./components/AboutMe.vue";
import SandboxProjects from "./components/SandboxProjects.vue";

export default {
  name: "App",
  components: {
    AboutMe,
    SandboxProjects,
  },
};
</script>

<style>
@import url("./normalize.css");
@import url(https://fonts.googleapis.com/css?family=Montserrat:100,200,300,regular,500,600,700,800,900,100italic,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic);
@import url(https://fonts.googleapis.com/css?family=Poppins:100,100italic,200,200italic,300,300italic,regular,italic,500,500italic,600,600italic,700,700italic,800,800italic,900,900italic);
@import url(https://fonts.googleapis.com/css?family=Poppins:100,100italic,200,200italic,300,300italic,regular,italic,500,500italic,600,600italic,700,700italic,800,800italic,900,900italic);
@import url(https://fonts.googleapis.com/css?family=Open+Sans:300,regular,500,600,700,800,300italic,italic,500italic,600italic,700italic,800italic);
@import url(//db.onlinewebfonts.com/c/05335ae3bda1ac59737d1e4ef83f97b6?family=PacificNorthwestRoughW04);

.wrapper {
  min-height: 100%;
  display: flex;
  flex-direction: column;
  overflow: clip;
  /* font-family: "Montserrat";
  font-family: "Open Sans"; */
  font-family: "PacificNorthwestRoughW04";
  font-style: normal;
  color: black;
}
._container {
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 15px;
}
.project__link-ghpages > figure,
.project__link-gh > figure {
  width: 200px;
  background-size: contain;
  height: 250px;
}
.project__link-ghpages > figure {
  background: url("./assets/icons/github-pages.webp");
}
.project__link-gh > figure {
  background: url("./assets/icons/GitHub.png");
}
</style>
