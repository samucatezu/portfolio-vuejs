<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio:
            "Desde criança, eu sou apaixonado por tecnologia e negócios. Aos 12 anos descobri o" +
            "universo do desenvolvimento de software e agora, mais experiente, adentrei na" +
            "universidade de minha sonhada área. Curso analise e desenvolvimento de sistemas na" +
            "Unip e sou técnico em contabilidade. Sou uma pessoa ambiciosa, extrovertida e" +
            "autodidata.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img
        src="https://github.com/samucatezu.png"
        class="rounded-xl w-96"
        alt=""
      />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="
          font-general-regular
          mb-4
          text-ternary-dark
          dark:text-ternary-light
          text-lg
        "
      >
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>
