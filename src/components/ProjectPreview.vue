<script setup>
  import ProjectPreviewComponent from '../components/ProjectPreviewComponent.vue'
</script>

<template>
  <div class="project-intro">
    <h2>A selection of what I have done</h2>
    <p>These projects are publicly visible and not covered under NDA</p>
  </div>
  
  <div class="project-previews">
      <ProjectPreviewComponent previewTitle="The Academy of European Swordsmanship" previewImage="./assets/swordsmanship.ca-600x320.png" siteUrl="https://swordsmanship.ca"/>
      <ProjectPreviewComponent previewTitle="The Raj Manek Mentorship Program" previewImage="./assets/mankementorship.com-600x320.png" siteUrl="https://manekmentorship.com"/>
  </div>
</template>
  
<style scoped>
.project-intro{
  text-align: center;
}

.project-previews {
      display:flex;
      column-gap:2rem;
      justify-content:center;
      margin-top:2rem;
  }

  @media(max-width:800px) {
      .project-previews {
          display:flex;
          flex-direction: column;
          row-gap:2rem;
          justify-content:center;
          margin-top:2rem;
          margin-left:-15px;
      }
  }
</style>
  