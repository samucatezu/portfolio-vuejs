
<template>
  <div class="flex justify-center items-center text-center">
    <div
      class="
        font-general-regular
        text-lg text-ternary-dark
        dark:text-ternary-light
      "
    >
      &copy; {{ copyrightDate }}.
      <a
        href="https://github.com/samucatezu/portfolio-vuejs"
        target="__blank"
        class="
          font-general-medium
          hover:underline hover:text-indigo-600
          dark:hover:text-indigo-300
          duration-500
        "
      >
        {{ projectName }}
      </a>
      . Desenvolvido por
      <a
        href="https://github.com/samucatezu"
        target="__blank"
        class="
          font-general-medium
          text-secondary-dark
          dark:text-secondary-light
          uppercase
          hover:underline hover:text-indigo-600
          dark:hover:text-indigo-300
          duration-500
        "
        >{{ author }}</a
      >
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      copyrightDate: new Date().getFullYear(),
      projectName: "Vue.js Portfolio",
      author: "Samucatezu",
    };
  },
};
</script>

<style lang="scss" scoped></style>
