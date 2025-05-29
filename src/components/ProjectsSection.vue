<template>
  <div class="projects">
    <div>
      <h1>Our projects</h1>
      <p>
        are very different in terms of priority, scale and complexity of
        implementation
      </p>
    </div>
    <div>
      <ul>
        <li v-for="(project, index) in projectsList" :key="index">
          <div>
            <h2>{{ project.name }}</h2>
            <p>{{ project.desc }}</p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectsSection",
  data() {
    return {
      projectsList: [
        {
          name: "Emergency Aid. WAR 2022.",
          desc: "providing food and medicine to the shelters and animals which lost their homes and families due to the war",
        },
        {
          name: "Non-commercial feed line",
          desc: "construction of industrial production base where food for shelters will be produced on a free basis",
        },
        {
          name: "Education and Control",
          desc: "lectures on communication, organisation and coordination of processes, control over the use of aid",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
