<template>
  <div id="app">
    <HeaderComponent />
    <main>
      <AboutSection />
      <SkillsSection />
      <ProjectsSection />
      <ContactSection />
    </main>
    <FooterComponent />
  </div>
  <div class="bubbles">
  <span></span>
  <span></span>
  <span></span>
</div>
<div class="bubbles">
  <span></span>
  <span></span>
  <span></span>
</div>
<div class="bubbles">
  <span></span>
  <span></span>
  <span></span>
</div>
<div class="bubbles">
  <span></span>
  <span></span>
  <span></span>
</div>
<div class="bubbles">
  <span></span>
  <span></span>
  <span></span>
</div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import AboutSection from "./components/AboutSection.vue";
import SkillsSection from "./components/SkillsSection.vue";
import ProjectsSection from "./components/ProjectsSection.vue";
import ContactSection from "./components/ContactSection.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  components: {
    HeaderComponent,
    AboutSection,
    SkillsSection,
    ProjectsSection,
    ContactSection,
    FooterComponent,
  },
};
</script>

<style>
/* 전역 스타일 추가 */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
main {
  padding: 20px;
}
.bubbles {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: -1;
}

.bubbles span {
  position: absolute;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: rgba(255, 182, 193, 0.8); /* 핑크색 */
  animation: bubble 10s infinite ease-in-out;
  opacity: 0;
}

.bubbles span:nth-child(1) {
  animation-delay: 0s;
  left: 10%;
  background: #ff6f91;
}
.bubbles span:nth-child(2) {
  animation-delay: 2s;
  left: 30%;
  background: #ffc5e1;
}
.bubbles span:nth-child(3) {
  animation-delay: 4s;
  left: 50%;
  background: #f9a1c8;
}

@keyframes bubble {
  0% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(-800px) translateX(200px);
    opacity: 0;
  }
}
</style>