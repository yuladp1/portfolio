<template>
  <div class="about-me">
    <div class="_container">
      <div class="about-me__wrapper">
        <div class="about-me__content">
          Hi! I am Julia Romanovska - <br />
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
  margin: 100px;
}
.about-me__content {
  display: flex;
  padding: 40px;
  font-size: 42px;
  font-weight: 600;
}
.about-me__links {
  padding: 40px;
  display: flex;
  flex-direction: column;
  color: white;
}
</style>
