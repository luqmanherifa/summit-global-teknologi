<template>
  <div class="home">
    <HeroSection />
    <AboutSection />
    <ProjectsSection />
    <SupportsSection />
    <TeamSection />
    <CitizensSection />
    <PartnersSection />
    <ContactSection />
  </div>
</template>

<script>
import HeroSection from "@/components/HeroSection.vue";
import AboutSection from "@/components/AboutSection.vue";
import ProjectsSection from "@/components/ProjectsSection.vue";
import SupportsSection from "@/components/SupportsSection.vue";
import TeamSection from "@/components/TeamSection.vue";
import CitizensSection from "@/components/CitizensSection.vue";
import PartnersSection from "@/components/PartnersSection.vue";
import ContactSection from "@/components/ContactSection.vue";

export default {
  name: "HomeView",
  components: {
    HeroSection,
    AboutSection,
    ProjectsSection,
    SupportsSection,
    TeamSection,
    CitizensSection,
    PartnersSection,
    ContactSection,
  },
};
</script>
