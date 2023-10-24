<template>
  <div>
    <div class="py-10">
      <AppHero />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardH class="bg-[#D094E5] mx-5 px-10 sm:ml-10 mt-10" />
      <CardW
        :name="nama"
        :image="image"
        class="bg-[#A3DCD4] mx-5 px-10 mt-10"
      />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardW class="bg-[#E8B89C] mx-5 px-10 mt-10" />
      <CardH class="bg-[#BDDFF9] mx-5 px-10 sm:ml-10 mt-10" />
    </div>
    <div class="py-12 mt-10 text-center">
      <div class="">
        <h1 class="text-5xl font-playpen font-bold text-[#025A4E]">
          In Proggres.
        </h1>
      </div>
      <div class="mt-8">
        <p>
          I'm passionate about crafting experiences that are engaging,
          accessible, and user-centric.
        </p>
      </div>
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardW class="bg-[#FFFFFF] mx-5 px-10 mt-10 text-[#1C1C1C]" />
      <CardH class="bg-[#1C1C1C] mx-5 px-10 sm:ml-10 mt-10 text-[#ffffff]" />
    </div>
  </div>
</template>
<script>
import AppHero from "~/components/AppHero.vue";
import CardW from "~/components/CardW.vue";
import CardH from "~/components/CardH.vue";
import image from "@/assets/img/resepKita.jpg";

export default {
  data() {
    return {
      image: image,
      nama: "Resep Kita",
    };
  },
  components: {
    AppHero,
    CardH,
    CardW,
  },
};
</script>
