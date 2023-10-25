<template>
  <div class="flex flex-col justify-center mx-auto space-y-4 overflow-x-hidden">
    <div class="flex flex-wrap my-2 marquee">
      <Skill
        class="m-1 sm:mx-2"
        v-for="(name, index) in shuffledNames"
        :name="name"
        :key="index"
      />
    </div>
    <div class="flex flex-wrap marquee2">
      <Skill
        v-for="(name, index) in shuffledNames"
        :name="name"
        :key="index"
        class="m-1 sm:mx-2"
      />
    </div>
  </div>
</template>

<script>
import Skill from "./skill.vue";
export default {
  data() {
    return {
      nama: ["HTML", "CSS", "Javascript", "Vue", "Nuxt Js", "Tailwind"],
      shuffledNames: [],
    };
  },
  mounted() {
    // Mulai perulangan untuk mengacak nama setiap beberapa detik
    this.shuffleNames(); // Pertama kali memanggil fungsi
    setInterval(this.shuffleNames, 10000); // Setiap 5 detik (sesuaikan dengan kebutuhan Anda)
  },
  methods: {
    shuffleNames() {
      const shuffled = [...this.nama].sort(() => Math.random() - 0.5);
      this.shuffledNames = shuffled;
    },
  },

  components: {
    Skill,
  },
};
</script>

<style>
@keyframes marquee {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}

.marquee {
  overflow: hidden;
  animation: marquee 10s linear infinite;
}

@keyframes marquee2 {
  0% {
    transform: translateX(-100%);
  }
  100% {
    transform: translateX(100%);
  }
}

.marquee2 {
  overflow: hidden;
  animation: marquee2 10s linear infinite;
}
</style>
