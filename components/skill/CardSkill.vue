<template>
  <div class="flex flex-col space-y-4 overflow-x-hidden">
    <div class="grid grid-flow-col gap-2 marquee">
      <Skill
        :name="nama[index % nama.length]"
        class="mx-2 sm:mx-4"
        v-for="index in 4"
        :key="index"
      />
    </div>
    <div class="grid grid-flow-col gap-2 mt-4 marquee2">
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
      nama: ["HTML", "CSS", "Javascript"],
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
  animation: marquee 20s linear infinite;
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
  animation: marquee2 20s linear infinite;
}
</style>
