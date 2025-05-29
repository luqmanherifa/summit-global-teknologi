<template>
  <div class="citizens">
    <div>
      <h1>Socially active citizens</h1>
      <p>support us</p>
    </div>
    <div>
      <ul>
        <li v-for="(citizen, index) in citizensList" :key="index">
          <div>
            <img src="" alt="" />
            <h2>{{ citizen.name }}</h2>
            <p>{{ citizen.job }}</p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "CitizensSection",
  data() {
    return {
      citizensList: [
        {
          photo: "",
          alt: "Oleksiy Tritenko",
          name: "Oleksiy Tritenko",
          job: "theater and film actor",
        },
        {
          photo: "",
          alt: "Stanislav Boklan",
          name: "Stanislav Boklan",
          job: "People's Artist of Ukraine",
        },
        {
          photo: "",
          alt: "Alexander Rudinsky",
          name: "Alexander Rudinsky",
          job: "theater and film actor",
        },
        {
          photo: "",
          alt: "Oksana Zhdanova",
          name: "Oksana Zhdanova",
          job: "theater and film actress",
        },
        {
          photo: "",
          alt: "Natalka Denisenko",
          name: "Natalka Denisenko",
          job: "theater and film actress",
        },
        {
          photo: "",
          alt: "Maksym Samchyk",
          name: "Maksym Samchyk",
          job: "theater and film actor",
        },
        {
          photo: "",
          alt: "Kateryna Vyshneva",
          name: "Kateryna Vyshneva",
          job: "theater and film actress",
        },
        {
          photo: "",
          alt: "Irma Vitovska",
          name: "Irma Vitovska",
          job: "Honored Actress of Ukraine",
        },
        {
          photo: "",
          alt: "Igor Portyanko",
          name: "Igor Portyanko",
          job: "actor of theater and cinema",
        },
        {
          photo: "",
          alt: "Dmytro Surzhikov",
          name: "Dmytro Surzhikov",
          job: "Honored Artist of Ukraine",
        },
        {
          photo: "",
          alt: "Daria Barihashvili",
          name: "Daria Barihashvili",
          job: "theater and film actress",
        },
        {
          photo: "",
          alt: "Vera Kobzar",
          name: "Vera Kobzar",
          job: "theater and film actress",
        },
        {
          photo: "",
          alt: "Andriy Fedynchyk",
          name: "Andriy Fedynchyk",
          job: "theater and film actor",
        },
        {
          photo: "",
          alt: "Anastasia Nesterenko",
          name: "Anastasia Nesterenko",
          job: "theater and film actress",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
