<script>
import AboutClientSingle from "./AboutClientSingle.vue";

export default {
  components: {
    AboutClientSingle,
  },
  data: () => {
    return {
      clientsHeading: "Algumas empresas que eu já trabalhei",
      clients: [
        {
          id: 1,
          title: "GBM",
          img: require("@/assets/images/brands/gbm.jpg"),
        },
        {
          id: 2,
          title: "GFT Technologies SE",
          img: require("@/assets/images/brands/gft_0_0.jpg"),
        },
      ],
    };
  },
};
</script>

<template>
  <div class="mt-10 sm:mt-20; allign-items: center">
    <p
      class="
        font-general-medium
        text-2xl
        sm:text-3xl
        text-primary-dark
        dark:text-primary-light
      "
    >
      {{ clientsHeading }}
    </p>
    <div
      class="
        grid grid-cols-2
        sm:grid-cols-4
        mt-10
        sm:mt-14
        gap-2;
        place-items-center
      "
    >
      <AboutClientSingle
        v-for="client in clients"
        :key="client.id"
        :client="client"
      />
    </div>
  </div>
</template>
