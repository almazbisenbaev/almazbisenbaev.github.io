<template>

    <div class="comingsoon">Portfolio will be here</div>
  
    <!-- <section id="portfolio" class="section ov-h pos-r">
      <div class="container">
        <div class="section-header">
          <h2 class="section-title">My portfolio</h2>
        </div>
      </div>
  
      <div class="container">
        <div class="case-line" v-for="(project, index) in projects" :key="index">
          <div class="case-line-intro">
            <div class="case-line-title">
              <a :href="project.url" target="_blank">{{ project.title }}</a>
            </div>
            <div class="case-line-details">
              <div>{{ project.year }}</div>
              <div>{{ project.skills }}</div>
              <div>
                For
                <a
                  :href="project.clientUrl"
                  target="_blank"
                  rel="noopener noreferrer"
                  >{{ project.client }}</a
                >
              </div>
            </div>
          </div>
          <div class="case-line-descr">{{ project.description }}</div>
        </div>
        <div
          class="divider divider-space"
          v-if="index < projects.length - 1"
        ></div>
      </div>
    </section> -->
  
  </template>
  
  <script lang="ts">
  import { defineComponent } from "vue";
  
  interface Project {
    title: string;
    url: string;
    year: number;
    skills: string;
    client: string;
    clientUrl: string;
    description: string;
  }
  
  export default defineComponent({
    name: "PortfolioSection",
    data() {
      return {
        projects: [
          {
            title: "muafaktur.de",
            url: "//muafaktur.de",
            year: 2023,
            skills: "UX Design, Development",
            client: "Mindlind",
            clientUrl: "//mindlind.de",
            description:
              "Designed in Figma, built with WordPress. Bespoke theme, WooCommerce.",
          },
          {
            title: "medienfaktur.com",
            url: "//medienfaktur.com",
            year: 2024,
            skills: "UX Design, Development",
            client: "Mindlind",
            clientUrl: "//mindlind.de",
            description: "Designed in Figma, built with WordPress.",
          },
        ] as Project[],
      };
    },
  });
  </script>
  