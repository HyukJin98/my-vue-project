<template>
    <section id="skills">
      <h2>My Skills</h2>
      <ul>
        <li v-for="skill in skills" :key="skill.name">
          <div class="skill-name">{{ skill.name }}</div>
          <div class="progress-bar">
            <div class="progress" :style="{ width: skill.percent + '%' }"></div>
          </div>
        </li>
      </ul>
    </section>
  </template>
  
  <script>
  export default {
    name: "SkillsSection",
    data() {
      return {
        skills: [
          { name: "HTML5", percent: 80 },
          { name: "CSS3", percent: 80 },
          { name: "JavaScript", percent: 70 },
          { name: "Vue.js", percent: 60 },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  #skills {
    padding: 20px;
  }
  .progress-bar {
    background: #e0e0e0;
    border-radius: 5px;
    height: 10px;
    margin: 5px 0;
    width: 100%;
  }
  .progress {
    background: #42b883;
    height: 100%;
    border-radius: 5px;
  }
  </style>
  