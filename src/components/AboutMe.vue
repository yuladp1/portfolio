<template>
  <div class="about-me">
    <div class="_container">
      <div class="about-me__wrapper">
        <div class="about-me__content">
          Hi! <br />
          I am Julia Romanovska - <br />
          super-puper developer!!! :)))))
        </div>
        <div class="about-me__links">
          <a href="">github</a>
          <a href="">linkedin</a>
          <a href="">something else</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.about-me {
  background: url("../assets/sandbox-images/background-with-gradient.webp");
  background-size: cover;
  color: white;
}
.about-me__wrapper {
  display: flex;
  margin: 50px 0;
  align-items: center;
  justify-content: center;
}
.about-me__content {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 87px;

  color: #ffffff;
}

.about-me__links {
  padding: 40px;
  display: flex;
  flex-direction: column;
  color: white;
}
</style>
