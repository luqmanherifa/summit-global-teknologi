<template>
  <div class="team">
    <div>
      <h1>Our team</h1>
      <p>
        consists of completely different people who are united by a common
        desire - to help
      </p>
    </div>
    <div>
      <ul>
        <li v-for="(team, index) in teamList" :key="index">
          <div>
            <img src="" alt="" />
            <h2>{{ team.name }}</h2>
            <p>{{ team.role }}</p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamSection",
  data() {
    return {
      teamList: [
        {
          photo: "",
          alt: "Daryna Deriy",
          name: "Daryna Deriy",
          role: "Chairman of the Board",
        },
        {
          photo: "",
          alt: "Polina Snisarenko-Kulchytska",
          name: "Polina Snisarenko-Kulchytska",
          role: "Curator of the Foundation",
        },
        {
          photo: "",
          alt: "Bohdan Kulchytsky",
          name: "Bohdan Kulchytsky",
          role: "Executive Manager",
        },
        {
          photo: "",
          alt: "Mykhaylo Deriy",
          name: "Mykhaylo Deriy",
          role: "Operation Manager",
        },
        {
          photo: "",
          alt: "Ksenia Nikishina",
          name: "Ksenia Nikishina",
          role: "Office manager",
        },
        {
          photo: "",
          alt: "Anna Andriychuk",
          name: "Anna Andriychuk",
          role: "SMM-manager",
        },
        {
          photo: "",
          alt: "Anastasia Kovalchuk",
          name: "Anastasia Kovalchuk",
          role: "Director",
        },
        {
          photo: "",
          alt: "Basil Gloo",
          name: "Basil Gloo",
          role: "Web Developer",
        },
        {
          photo: "",
          alt: "Lina Yakobchuk",
          name: "Lina Yakobchuk",
          role: "Designer",
        },
        {
          photo: "",
          alt: "Anastasia Yevchenko",
          name: "Anastasia Yevchenko",
          role: "Translator",
        },
        {
          photo: "",
          alt: "Office Manager",
          name: "Office Manager",
          role: "open vacancy",
        },
        {
          photo: "",
          alt: "SEO specialist",
          name: "SEO specialist",
          role: "open vacancy",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
