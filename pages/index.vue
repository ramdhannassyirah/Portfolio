<template>
  <div class="min-h-screen">
    <div class="py-10">
      <AppHero />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardH
        :name="nama[4]"
        :image="images[4]"
        :href="url[2]"
        class="bg-[#D094E5] mx-5 px-10 sm:ml-10 mt-10"
        v-motion-slide-visible-left
      />
      <CardW
        :name="nama[0]"
        :image="images[0]"
        :href="url[0]"
        class="bg-[#A3DCD4] mx-5 px-5 sm:px-10 mt-10"
        v-motion-slide-visible-right
      />
    </div>
    <div class="flex flex-wrap items-center justify-center">
      <CardW
        :name="nama[1]"
        :image="images[1]"
        class="bg-[#E8B89C] mx-5 px-10 mt-10"
        v-motion-slide-visible-left
      />
      <CardH
        :name="nama[3]"
        :image="images[3]"
        :href="url[1]"
        class="bg-[#BDDFF9] mx-5 px-10 sm:ml-10 mt-10"
        v-motion-slide-visible-right
      />
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
      <CardW
        :name="nama[2]"
        :image="images[2]"
        class="bg-[#FFFFFF] mx-5 px-10 mt-10 text-[#1C1C1C]"
        v-motion-slide-visible-left
      />
      <CardH
        class="bg-[#1C1C1C] mx-5 px-10 sm:ml-10 mt-10 text-[#ffffff] animate__bounceInRight"
        v-motion-slide-visible-right
      />
    </div>
  </div>
</template>
<script>
import AppHero from "~/components/AppHero.vue";
import CardW from "~/components/Card/CardW.vue";
import CardH from "~/components/Card/CardH.vue";
import resepKita from "@/assets/img/resepKita.jpg";
import portfolio from "@/assets/img/protfolio.jpg";
import farmWeb from "@/assets/img/FarmTech.jpg";
import agency from "@/assets/img/agency.jpg";
import company from "@/assets/img/company-2.jpg";
import {css, html, vue, js, tailwind, nuxt} from "@/store/import.js";

export default {
  data() {
    return {
      images: [resepKita, portfolio, farmWeb, agency, company],
      nama: ["Resep Kita", "Portfolio", "FarmTech", "Agency", "LiTechProfile"],
      url: [
        "https://resep-kitav1.netlify.app/",
        "https://agency-website-wheat.vercel.app/",
        "https://li-tech-profile.vercel.app/",
      ],
      logo: [css, html, vue, js, tailwind, nuxt],
    };
  },
  components: {
    AppHero,
    CardH,
    CardW,
  },
};
</script>
