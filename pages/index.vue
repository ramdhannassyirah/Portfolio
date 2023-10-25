<template>
  <div>
    <div class="py-10">
      <AppHero />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardH class="bg-[#D094E5] mx-5 px-10 sm:ml-10 mt-10" />
      <CardW
        :name="nama[0]"
        :image="images[0]"
        :href="url"
        class="bg-[#A3DCD4] mx-5 px-5 sm:px-10 mt-10"
      />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardW
        :name="nama[1]"
        :image="images[1]"
        class="bg-[#E8B89C] mx-5 px-10 mt-10"
      />
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
import CardW from "~/components/Card/CardW.vue";
import CardH from "~/components/Card/CardH.vue";
import resepKita from "@/assets/img/resepKita.jpg";
import portfolio from "@/assets/img/protfolio.jpg";

export default {
  data() {
    return {
      images: [resepKita, portfolio],
      nama: ["Resep Kita", "Portfolio"],
      url: ["https://resep-kitav1.netlify.app/"],
    };
  },
  components: {
    AppHero,
    CardH,
    CardW,
  },
};
</script>
