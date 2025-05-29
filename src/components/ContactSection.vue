<template>
  <div class="contact">
    <div>
      <h1>Contact us</h1>
      <p>Kyiv, Ukraine</p>
      <p>mail@isa.co.ua</p>
    </div>
    <ul>
      <li v-for="(link, index) in socialLinks" :key="index">
        <a :href="link.href" target="_blank" rel="noopener">{{ link.name }}</a>
      </li>
    </ul>
    <img src="" alt="" />
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

<style scoped lang="scss"></style>
