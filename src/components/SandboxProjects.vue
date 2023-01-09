<template>
  <div class="sandbox__wrapper sandbox">
    <h2 class="sandbox__title">Sandbox</h2>
    <div class="sandbox__projects projects _container">
      <div class="projects__project project">
        <figure class="project__image">
          <img src="../assets/projects-image/growfy.png" alt="" />
        </figure>
        <div class="project__content">
          <h2>Project 1</h2>
          <p class="project__overview">rfrjq kdjfkdjfkjdfksjdfkjkfjsdkfjskdjfhsk</p>
          <a href="" class="project__link">Link to project</a>
        </div>
      </div>
      <div class="projects__project project">
        <figure class="project__image">
          <img src="../assets/projects-image/relvise.png" alt="" />
        </figure>
        <div class="project__content">
          <h2>Project 1</h2>
          <p class="project__overview">rfrjq kdjfkdjfkjdfksjdfkjkfjsdkfjskdjfhsk</p>
          <a href="" class="project__link">Link to project</a>
        </div>
      </div>
      <div class="projects__project project">
        <figure class="project__image">
          <img src="../assets/projects-image/crypto.png" alt="" />
        </figure>
        <div class="project__content">
          <h2>Project 1</h2>
          <p class="project__overview">rfrjq kdjfkdjfkjdfksjdfkjkfjsdkfjskdjfhsk</p>
          <a href="" class="project__link">Link to project</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SandboxProjects",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.sandbox {
}
.sandbox__title {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 54px;

  color: #4d533c;
}
.sandbox__projects {
}
.projects {
}
.projects > div:not(:last-child) {
  margin-bottom: 200px;
}
.projects > div:nth-child(2n) {
  flex-direction: row-reverse;
}
.projects__project {
}
.project {
  padding: 0;
  display: flex;
  grid: 20px;
  align-items: center;
  justify-content: space-evenly;
}
.project__image {
  flex: 0 1 50%;
}
.project__image img {
  object-fit: cover;
  width: 100%;
}
.project__content {
  display: flex;
  flex-direction: column;
  gap: 30px;
  align-items: center;
}
.project__content h2,
.project__overview,
.project__link {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 36px;
  line-height: 111.5%;
  /* or 40px */

  letter-spacing: -0.025em;
  color: black;
}
.project__overview {
  flex: 0 1 50%;
  font-size: 16px;
  line-height: 26px;
  /* or 162% */
  text-align: center;
}
.project__link {
  padding: 20px 50px;
  text-align: center;
  border: 1px solid black;
  font-size: 18px;
  text-transform: uppercase;
  background: white;
}
</style>
