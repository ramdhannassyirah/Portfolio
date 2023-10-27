<template>
  <button
    v-if="showButton"
    @click="scrollToTop"
    class="fixed px-4 py-2 text-white bg-blue-500 rounded-full bottom-5 right-5 hover:bg-blue-700"
  >
    Scroll to Top
  </button>
</template>

<script>
export default {
  data() {
    return {
      showButton: false,
    };
  },
  created() {
    window.addEventListener("scroll", this.toggleButton);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.toggleButton);
  },
  methods: {
    toggleButton() {
      this.showButton = window.scrollY > 300;
    },
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>
