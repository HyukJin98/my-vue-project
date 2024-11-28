<template>
    <section id="projects">
      <h2>Projects</h2>
      <div class="projects-grid">
        <div class="project" v-for="project in projects" :key="project.name">
          <h3>{{ project.name }}</h3>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank">View Demo</a>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "ProjectsSection",
    data() {
      return {
        projects: [
          {
            name: "개인 프로젝트",
            description: "커뮤니티 웹사이트",
            link: "https://github.com/HyukJin98/Project",
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
  }
  .project {
    border: 1px solid #ccc;
    padding: 10px;
    text-align: center;
  }
  </style>
  