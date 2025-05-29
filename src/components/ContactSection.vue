<template>
  <div class="contact">
    <div class="contact__info">
      <h1 class="contact__title">Contact us</h1>
      <p class="contact__location">Kyiv, Ukraine</p>
      <p class="contact__email">mail@isa.co.ua</p>
      <ul class="contact__social-list">
        <li
          class="contact__social-item"
          v-for="(link, index) in socialLinks"
          :key="index"
        >
          <a
            class="contact__social-link"
            :href="link.href"
            target="_blank"
            rel="noopener"
          >
            {{ link.name }}
          </a>
        </li>
      </ul>
    </div>
    <div>
      <img
        class="contact__image"
        src="../assets/images/contactStarAnimals.svg"
        alt="Star with animals illustration"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactSection",
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
.contact {
  display: flex;
  flex-direction: row;
  background-color: #31be32;
  padding: 9rem;
  text-align: left;
  color: #000000;

  &__info {
    flex: 1;
  }

  &__title {
    font-size: 3.2rem;
  }

  &__location,
  &__email {
    font-size: 2.2rem;
  }

  &__social-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 1rem;
    padding: 0;
  }

  &__image {
    width: 540px;
    height: auto;
  }
}
</style>
