<template>
  <div class="flex flex-col space-y-4 overflow-x-hidden">
    <div class="flex marquee">
      <Skill
        :name="nama[index % nama.length]"
        class="sm:mx-4"
        v-for="index in 4"
        :key="index"
      />
    </div>
    <div class="flex marquee2">
      <Skill
        :name="nama[(index + 1) % nama.length]"
        class="sm:mx-4"
        v-for="index in 4"
        :key="index"
      />
    </div>
  </div>
</template>

<script>
import Skill from "./skill.vue";
export default {
  data() {
    return {
      nama: ["HTML", "CSS", "Javascript", "Vue", "Nuxt Js", "Tailwind CSS"],
    };
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
