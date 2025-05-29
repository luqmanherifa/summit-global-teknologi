<template>
  <div class="supports">
    <div>
      <h1>We want to help</h1>
      <p>
        homeless packs, volunteers, guardians, overstayers, shelters and other
        organisations
      </p>
    </div>
    <div>
      <ul>
        <li v-for="(support, index) in supportsList" :key="index">
          <div>
            <h2>{{ support.name }}</h2>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "SupportsSection",
  data() {
    return {
      supportsList: [
        { name: "Shelter of Victoria Bulbyna" },
        { name: "City of faithful hearts" },
        { name: "Shelter of Natalia Tymoshenko" },
        { name: "Shelter of Jeanne Sass" },
        { name: "Shelter of Victoria Bondarenko" },
        { name: "Sterilization center" },
        { name: "Zoo chance" },
        { name: "Save lives" },
        { name: "City Center for the Treatment of Animals" },
        { name: "Society for the Protection of Animals in Sumy" },
        { name: "The right to life" },
        { name: "4 paws" },
        { name: "The kingdom of cats" },
        { name: "Zvir" },
        { name: "Mercy" },
        { name: "Happy dog" },
        { name: "Give me a paw, friend" },
        { name: "Friend" },
        { name: "Hope" },
        { name: "We are for the right to life" },
        { name: "Planeta" },
        { name: "Second Life" },
        { name: "Happy shore" },
        { name: "Retrieverteam" },
        { name: "Shelter of Irina Dobrolyubova" },
        { name: "Matilda" },
        { name: "Life" },
        { name: "Second chance" },
        { name: "SOS" },
        { name: "Best friends" },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
