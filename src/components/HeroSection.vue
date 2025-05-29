<template>
  <div class="hero">
    <div class="hero__header">
      <img
        src="../assets/images/heroDog.svg"
        alt="ISA Logo Dog"
        class="hero__logo"
      />
      <h1 class="hero__title">Innovative Solutions for Animals</h1>
    </div>
    <p class="hero__subtitle">charity organization</p>
    <ul class="hero__socials">
      <li
        v-for="(link, index) in socialLinks"
        :key="index"
        class="hero__social-item"
      >
        <a
          :href="link.href"
          target="_blank"
          rel="noopener"
          class="hero__social-link"
          >{{ link.name }}</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HeroSection",
  data() {
    return {
      socialLinks: [
        {
          name: "youtube",
          href: "https://www.youtube.com/channel/UCflad3HMzVzumevfDEqJFFQ/featured",
        },
        {
          name: "instagram",
          href: "https://www.instagram.com/isa.official.ua/",
        },
        { name: "facebook", href: "https://www.facebook.com/isa.co.ua" },
        { name: "patreon", href: "https://www.patreon.com/isa_co_ua" },
        { name: "telegram", href: "https://t.me/isa_co_ua" },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.hero {
  background-color: #fcf944;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 600px;
  color: #000000;

  &__header {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 2rem;
  }

  &__logo {
    width: 200px;
    height: auto;
  }

  &__title {
    font-size: 3.5rem;
    width: 300px;
    line-height: 1;
    text-align: left;
  }

  &__subtitle {
    font-size: 2rem;
    margin-top: 1rem;
  }

  &__socials {
    list-style: none;
    display: flex;
    flex-direction: row;
    gap: 1rem;
    margin-top: 1rem;
  }

  &__social-link {
    font-size: 1.5rem;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
}
</style>
