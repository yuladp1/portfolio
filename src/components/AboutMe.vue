<template>
  <div class="about-me">
    <div class="about-me__wrapper">
      <transition @before-enter="beforenter" @enter="enter" appear>
        <div class="about-me__content">
          <span> Julia </span>
          <span> Romanovska</span>
          <p>
            fhdjfh dfhskjdfhsdjfhdjfhd djfskdjfksjd fksjdfhdjf hjdfhjdfhjdhfjd fjdhfjdhfjd
            hfjdh jhghf
          </p>
        </div>
      </transition>

      <div class="about-me__links">
        <transition @before-enter="beforenterLink" @enter="enterLink" appear>
          <a href="https://github.com/yuladp1" target="_blank">github</a>
        </transition>
        <transition @before-enter="beforenterLink" @enter="enterLink" appear>
          <a href="www.linkedin.com/in/julia-romanovska" target="_blank">linkedin</a>
        </transition>
      </div>
    </div>
  </div>
</template>

<script>
import gsap from "gsap";
export default {
  name: "AboutMe",
  created() {},
  data() {
    return {
      quotes: [],
    };
  },
  props: {},
  methods: {
    beforenter(el) {
      el.style.opacity = "0";
      gsap.from(el, {
        color: "blue",
        fontSize: "1rem",
      });
    },
    enter(el) {
      gsap.to(el, {
        opacity: 1,
        duration: 1,
        fontSize: "6.25rem",
      });
    },
    beforenterLink(el) {
      gsap.from(el, {
        opacity: 0,
        y: +100,
      });
    },
    enterLink(el) {
      gsap.to(el, {
        opacity: 1,
        duration: 1,
        y: 0,
      });
    },
  },
};
</script>

<style scoped>
@import url(//db.onlinewebfonts.com/c/05335ae3bda1ac59737d1e4ef83f97b6?family=PacificNorthwestRoughW04);
@import url(//db.onlinewebfonts.com/c/a4745f4b1d04fa025c6a05d891ed0126?family=Monument+Extended+Ultrabold);
.about-me {
  /*font-family: "PacificNorthwestRoughW04"; */
  font-family: "Monument Extended Ultrabold";
  letter-spacing: 5px;
  text-transform: uppercase;
  font-size: 6.25rem;
  line-height: 8rem;
  background: url("../assets/about-me-images/background.png");
  background-size: cover;
  color: white;
  height: 470px;
}
.about-me__wrapper {
  display: flex;
  flex-direction: column;
  gap: 40px;
  margin: 50px 0;
  align-items: center;
  justify-content: center;
  background: rgba(2, 14, 12, 0.01);
  backdrop-filter: blur(10px);
  border-radius: 10px;
  padding: 50px;
  margin: 130px;
  -webkit-box-shadow: 16px 16px 12px 0px rgb(9 9 9 / 20%);
  -moz-box-shadow: 16px 16px 12px 0px rgba(9, 9, 9, 0.2);
  box-shadow: 16px 16px 12px 0px rgb(9 9 9 / 20%);
  border: 1px solid white;
}
.about-me__content {
  flex: 0 1 60%;
  text-shadow: -0 -2px 5px #000000, 0 -2px 5px #000000, -0 2px 5px #000000,
    0 2px 5px #000000, -2px -0 5px #000000, 2px -0 5px #000000, -2px 0 5px #000000,
    2px 0 5px #000000, -1px -2px 5px #000000, 1px -2px 5px #000000, -1px 2px 5px #000000,
    1px 2px 5px #000000, -2px -1px 5px #000000, 2px -1px 5px #000000, -2px 1px 5px #000000,
    2px 1px 5px #000000, -2px -2px 5px #000000, 2px -2px 5px #000000, -2px 2px 5px #000000,
    2px 2px 5px #000000, -2px -2px 5px #000000, 2px -2px 5px #000000, -2px 2px 5px #000000,
    2px 2px 5px #000000;
  display: flex;
  flex-direction: column;
}
.about-me__content > p {
  font-family: "Poppins";
  font-size: 1.5rem;
  line-height: 2.5rem;
  text-transform: none;
  text-shadow: none;
  color: black;
}
.about-me__links {
  font-size: 32px;
  display: flex;
  /* color: white; */
  gap: 20px;
  align-items: center;
  justify-content: flex-start;
}
.about-me__links > a {
  color: white;
  background: #02181f;
  border: 1px solid #02181f;
  box-shadow: 0px 4px 67px rgb(1 2 17 / 60%);
  border-radius: 10px;
  padding: 10px 30px;
  font-size: 1.5rem;
  line-height: 2rem;
}
.about-me__links > a:hover {
  color: #02181f;
  background: white;

  border: 1px solid #02181f;
}
</style>
