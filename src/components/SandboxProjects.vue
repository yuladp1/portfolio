<template>
  <div class="sandbox__wrapper sandbox">
    <h2 class="sandbox__title _title">Projects</h2>
    <section class="sandbox__projects projects _container">
      <div class="projects__project project">
        <figure class="project__image" v-motion-slide-visible-left>
          <img src="../assets/projects-image/growfy.png" alt="" />
        </figure>
        <div class="project__content">
          <h2 class="project__content-title" v-motion-pop-visible>Project GROWFY</h2>
          <p class="project__overview">Landing page</p>
          <div class="project__links">
            <a href="https://yuladp1.github.io/growfy/" class="project__link-ghpages" v-motion-pop-visible>
              go live page</a
            >
            <a href="https://github.com/yuladp1/growfy" class="project__link-gh" v-motion-pop-visible> Code</a>
          </div>
        </div>
      </div>
      <div class="projects__project project">
        <figure class="project__image" v-motion-slide-visible-left>
          <img src="../assets/projects-image/relvise.png" alt="" />
        </figure>
        <div class="project__content">
          <h2 class="project__content-title">Project RELVISE</h2>
          <p class="project__overview">rfrjq kdjfkdjfkjdfksjdfkjkfjsdkfjskdjfhsk</p>
          <div class="project__links">
            <a
              href="https://yuladp1.github.io/relvise-vue/"
              class="project__link-ghpages"
              v-motion-pop-visible
            >
              <span>go live page</span></a
            >
            <a href="https://github.com/yuladp1/relvise-vue" class="project__link-gh" v-motion-pop-visible>
              <span>Code</span></a
            >
          </div>
        </div>
      </div>
      <div class="projects__project project">
        <figure class="project__image" v-motion-slide-visible-left>
          <img src="../assets/projects-image/crypto.png" alt="" />
        </figure>
        <div class="project__content">
          <h2 class="project__content-title">Project CRYPTO</h2>
          <p class="project__overview">rfrjq kdjfkdjfkjdfksjdfkjkfjsdkfjskdjfhsk</p>
          <div class="project__links">
            <a href="https://yuladp1.github.io/crypto-vue/" class="project__link-ghpages" v-motion-pop-visible>
              go live page</a
            >
            <a href="https://github.com/yuladp1/crypto-vue" class="project__link-gh" v-motion-pop-visible>
              Code</a
            >
          </div>
        </div>
      </div>
    </section>
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
  padding-top: 150px;
}
.sandbox__projects {
}
.projects {
}
.projects > div:not(:last-child) {
  margin-bottom: 100px;
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
  border: 2px solid grey;
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
.project__content-title,
.project__overview,
.project__links {
  display: flex;
  gap: 20px;
}
.project__links > a {
  flex: 0 1 50%;
  padding: 20px 30px;
  border: 2px solid black;
}

.project__content-title {
  text-align: center;
  font-style: normal;
  font-weight: 700;
  font-size: 2rem;
  line-height: 87px;
}
.project__overview {
  flex: 0 1 50%;
  text-align: center;

  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 32px;
}

.project__link-gh > span:before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  background-image: url(http://localhost:8080/img/icon-github.31a9cfe3.png);
  background-size: cover;
  width: 80px;
  height: 80px;
}
</style>
