<template>
  <div class="container mx-auto">
    <div
      class="container mx-auto grid grid-cols-1 mt-10 sm:grid-cols-2 justify-items-center"
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
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            natus dignissimos asperiores illum. Harum, nihil! Eaque perferendis
            consequatur similique eligendi.
          </p>
        </div>
      </div>
    </div>
    <!-- components skill -->
    <skill />
    <div class="grid justify-items-center sm:w-[700px] mt-10 px-4 sm:ml-80">
      <h1 class="text-xl sm:text-5xl font-bold font-playpen text-[#025A4E]">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur
        aperiam ducimus cumque dicta expedita possimus!
      </h1>

      <p class="mt-5">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nesciunt,
        autem laborum deleniti perferendis numquam eveniet natus mollitia non
        rem vitae?
      </p>
    </div>
  </div>
</template>
<script>
import skill from "~/components/skill.vue";
export default {
  components: {
    skill,
  },
};
</script>
