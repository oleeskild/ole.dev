<template>
  <div>
    <h2>Stuff I've made</h2>
    <div class="project-list">
    <project-card
        :title="'Obsidian Digital Garden'"
        :url="' https://dg-docs.ole.dev/'"
        :icon="'&#x1F3E1;'"
      >
      </project-card>
      <project-card
        :title="'Talks'"
        :url="' https://notes.ole.dev/foredrag/'"
        :icon="'&#x1F5E3;'"
      >
      </project-card>
      <project-card
        :title="'gurl'"
        :url="' https://gurl.ole.dev/'"
        :icon="'&#x1F517;'"
      >
        </project-card>
    <project-card
        :title="'Digital Hage'"
        :url="' https://notes.ole.dev/'"
        :icon="'&#x1F331;'"
      >
      </project-card>
       <project-card
        :title="'Bergens Røst'"
        :url="'https://bergensrost.ole.dev'"
        :icon="'&#x26f0;'"
      >
      </project-card>
      <project-card
        :title="'Jam Docs'"
        :url="'https://ole.dev/jam'"
        :icon="'&#x1F36F;'"
      >
      </project-card>
      <project-card
        :title="'Foos Invitation'"
        :url="'https://foosinvite.netlify.app/'"
        :icon="'&#x26bd;'"
      >
      </project-card>
       <project-card
        :title="'NFT Gallery'"
        :url="'https://ole.dev/nft'"
        :icon="'&#x1F5BC;'"
      >
      </project-card>
      <project-card
        :title="'Middag'"
        :url="'https://ole.dev/middag'"
        :icon="'&#x1F354;'"
      >
      </project-card>
      <project-card
        :title="'Riddlr'"
        :url="'https://ole.dev/riddlr'"
        :icon="'&#x1F3A9;'"
      >
      </project-card>
      <project-card
        :title="'Daily Dash'"
        :url="'https://ole.dev/dash'"
        :icon="'&#x1F39B;'"
      >
      </project-card>
    </div>
  </div>
</template>
<script>
import ProjectCard from "./ProjectCard.vue";
export default {
  components: {
    ProjectCard,
  },
};
</script>
<style scoped>
.project-list {
  display: grid;
  grid-template-columns: 50% 50%;
  grid-template-rows: auto;
  column-gap: 10px;
  margin-bottom: 20px;
}
h2 {
  text-align: center;
}
@media (max-width: 1024px) {
  .project-list {
    grid-template-columns: auto;
  }
}
</style>
