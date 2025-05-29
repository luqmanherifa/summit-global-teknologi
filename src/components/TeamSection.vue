<template>
  <div class="team">
    <div class="team__header">
      <h1 class="team__title">Our team</h1>
      <p class="team__description">
        consists of completely different people who are united by a common
        desire - to help
      </p>
    </div>
    <div class="team__list-wrapper">
      <ul class="team__list">
        <li class="team__item" v-for="(team, index) in teamList" :key="index">
          <div class="team__card">
            <img :src="team.photo" :alt="team.alt" class="team__photo" />
            <h2 class="team__name">{{ team.name }}</h2>
            <p class="team__role">{{ team.role }}</p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import teamDaryna from "@/assets/images/teamDaryna.jpg";
import teamPolina from "@/assets/images/teamPolina.jpg";
import teamBohdan from "@/assets/images/teamBohdan.jpg";
import teamMykhaylo from "@/assets/images/teamMykhaylo.jpg";
import teamKsenia from "@/assets/images/teamKsenia.jpg";
import teamAnna from "@/assets/images/teamAnna.jpg";
import teamAnastasia from "@/assets/images/teamAnastasia.jpg";
import teamBasil from "@/assets/images/teamBasil.png";
import teamLina from "@/assets/images/teamLina.jpg";
import teamYevchenko from "@/assets/images/teamYevchenko.jpg";
import teamOffice from "@/assets/images/teamOffice.svg";
import teamSeo from "@/assets/images/teamSeo.svg";

export default {
  name: "TeamSection",
  data() {
    return {
      teamList: [
        {
          photo: teamDaryna,
          alt: "Daryna Deriy",
          name: "Daryna Deriy",
          role: "Chairman of the Board",
        },
        {
          photo: teamPolina,
          alt: "Polina Snisarenko-Kulchytska",
          name: "Polina Snisarenko-Kulchytska",
          role: "Curator of the Foundation",
        },
        {
          photo: teamBohdan,
          alt: "Bohdan Kulchytsky",
          name: "Bohdan Kulchytsky",
          role: "Executive Manager",
        },
        {
          photo: teamMykhaylo,
          alt: "Mykhaylo Deriy",
          name: "Mykhaylo Deriy",
          role: "Operation Manager",
        },
        {
          photo: teamKsenia,
          alt: "Ksenia Nikishina",
          name: "Ksenia Nikishina",
          role: "Office manager",
        },
        {
          photo: teamAnna,
          alt: "Anna Andriychuk",
          name: "Anna Andriychuk",
          role: "SMM-manager",
        },
        {
          photo: teamAnastasia,
          alt: "Anastasia Kovalchuk",
          name: "Anastasia Kovalchuk",
          role: "Director",
        },
        {
          photo: teamBasil,
          alt: "Basil Gloo",
          name: "Basil Gloo",
          role: "Web Developer",
        },
        {
          photo: teamLina,
          alt: "Lina Yakobchuk",
          name: "Lina Yakobchuk",
          role: "Designer",
        },
        {
          photo: teamYevchenko,
          alt: "Anastasia Yevchenko",
          name: "Anastasia Yevchenko",
          role: "Translator",
        },
        {
          photo: teamOffice,
          alt: "Office Manager",
          name: "Office Manager",
          role: "open vacancy",
        },
        {
          photo: teamSeo,
          alt: "SEO specialist",
          name: "SEO specialist",
          role: "open vacancy",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.team {
  display: flex;
  flex-direction: column;
  background-color: #ffffff;
  padding: 9rem;
  text-align: left;
  color: #000000;
  gap: 3rem;

  &__title {
    font-size: 3.2rem;
  }

  &__description {
    font-size: 2.2rem;
    line-height: 1.5;
    margin-top: 1rem;
  }

  &__list-wrapper {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
  }

  &__list {
    padding: 0;
    gap: 3.2rem;
    display: flex;
    flex-wrap: wrap;
  }

  &__item {
    display: flex;
    justify-content: center;
  }

  &__card {
    background-color: #fcf944;
    border: 3px solid #000000;
    text-align: center;
    padding: 1.6rem;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  &__photo {
    width: 170px;
    height: 170px;
    filter: grayscale(100%);
  }

  &__name {
    font-size: 1.25rem;
    font-weight: 500;
    margin-top: 2rem;
    width: 170px;
  }

  &__role {
    font-size: 1rem;
    margin-top: 0.8rem;
    width: 170px;
  }
}
</style>
