<template>
  <div class="flex flex-col space-y-4 overflow-x-hidden">
    <div class="marquee grid grid-flow-col auto-cols-max">
      <skill class="mx-2 sm:mx-4" /> <skill class="mx-2 sm:mx-4" />
      <skill class="mx-2 sm:mx-4" /><skill class="mx-2 sm:mx-4" />
    </div>
    <div class="marquee2 grid grid-flow-col auto-cols-max mt-4">
      <skill class="mx-2 sm:mx-4" /> <skill class="mx-2 sm:mx-4" />
      <skill class="mx-2 sm:mx-4" /><skill class="mx-2 sm:mx-4" />
      <skill class="mx-2 sm:mx-4" />
    </div>
  </div>
</template>

<script>
import skill from "./skill.vue";
export default {
  components: {
    skill,
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

components: { skill },
