<template>
  <div class="partners">
    <div>
      <h1>Our partners</h1>
      <p>are take care of our fund and help us with many questions</p>
    </div>
    <div>
      <ul>
        <li v-for="(partner, index) in partnersList" :key="index">
          <div>
            <img src="" alt="" />
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "PartnersSection",
  data() {
    return {
      citizensList: [
        {
          image: "Logo-adviRES",
        },
        {
          image: "ovid-wind-logo",
        },
        {
          image: "TBS Industry",
        },
        {
          image: "Accurl",
        },
        {
          image: "Laudis",
        },
        {
          image: "Kickbite",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss"></style>
