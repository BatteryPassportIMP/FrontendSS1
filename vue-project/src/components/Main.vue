<script setup>
import AppFooter from "../components/AppFooter.vue";
import ProjectTab from "./ProjectTab.vue";
import Welcome from "./Welcome.vue";
import Team from "./Team.vue";
import Results from "./Results.vue";
import Learnings from "./Learnings.vue";
</script>
import Welcome from "./Welcome.vue";

<script>
  export default {
    data() {
        return {
            tab: "home",
            items: [
                "home",
                "project",
                "team",
                "results",
                "learnings",
                "contact"
            ],
        };
    },
}
</script>

<template>
  <VApp>
    <v-app-bar
        app
        color="#27ae5f"
      >
        <template v-slot:prepend>
            <v-app-bar-nav-icon to="">
                <img style="width:100%" src="../assets/logo_logo.png"/>
            </v-app-bar-nav-icon>
        </template>

        <v-app-bar-title
          class="text-white"
        >Econnovator</v-app-bar-title>

        <template v-slot:append>
            <v-tabs
              v-model="tab"
              class="text-white"
            >
              <v-tab value="home">Home</v-tab>
              <v-tab value="project">Project</v-tab>
              <v-tab value="team">Team</v-tab>
              <v-tab value="results">Results</v-tab>
              <v-tab value="learnings">Learnings</v-tab>
              <v-tab value="contact">Contact us</v-tab>
            </v-tabs>
        </template>
      </v-app-bar>
    <v-window v-model="tab" class="body">
      <v-window-item
        value="home"
      >
        <Welcome />
      </v-window-item>
      <v-window-item
        value="project"
      >
        <ProjectTab />
      </v-window-item>
      <v-window-item
        value="team">
        <Team />
      </v-window-item>
      <v-window-item
        value="results">
        <Results />
      </v-window-item>
      <v-window-item
        value="learnings">
        <Learnings />
      </v-window-item>
      <v-window-item
        value="contact">
      </v-window-item>
    </v-window>
    <AppFooter />
    </VApp>
</template>

<style>
.body {
  margin-top: 5%;
  margin-right: 5%;
  margin-left: 5%;
}

.heading {
  font-weight: bold;
  color: #00421A;
}

.battery-image {
  margin-top: 55%;
  margin-right: 10%;
}
</style>
