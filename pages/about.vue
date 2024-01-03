<template>
  <div class="container box-border mx-auto">
    <div
      class="container grid grid-cols-1 mx-auto mt-10 sm:grid-cols-2 justify-items-center"
    >
      <div class="text-center sm:hidden">
        <h1 class="text-4xl sm:text-5xl font-bold font-playpen text-[#025A4E]">
          I'm Ramdhan
        </h1>
      </div>
      <div
        class="mt-10 w-80 h-[400px] sm:w-96 sm:h-400 bg-[#AF937B] rounded-t-[80px] overflow-hidden"
      >
        <img src="../assets/img/rn.png" alt="" />
      </div>
      <div class="px-4 mt-10">
        <h1 class="text-xl sm:text-5xl font-bold font-playpen text-[#025A4E]">
          I'm a Web Developer working remotely from Cianjur, Indonesia.
        </h1>
        <div class="mt-4 sm:mt-6">
          <p class="text-xl font-roboto">
            "I am a Remote Web Developer with 1 year of experience, based in
            Cianjur, Indonesia. I specialize in developing various web solutions
            and applications with an emphasis on quality and efficiency. I have
            experience collaborating online, creating engaging user experiences,
            and tackling technical challenges in a remote working environment."
          </p>
        </div>
      </div>
    </div>
    <div class="my-[100px] text-center">
      <h1 class="text-2xl sm:text-5xl font-bold font-playpen text-[#025A4E]">
        Skills
      </h1>
      <!-- components Card skill -->
      <CardSkill />
    </div>
    <!-- descrption -->
    <Desc class="" />
  </div>
</template>
<script>
import Desc from "~/components/Desc.vue";
import CardSkill from "~/components/skill/CardSkill.vue";

export default {
  components: {
    CardSkill,
    Desc,
  },
};
</script>
