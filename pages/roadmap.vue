<template>
  <div
    class="grid items-center min-h-screen grid-flow-row justify-items-center"
  >
    <div class="my-5">
      <h1 class="text-3xl font-bold text-center font-playpen text-[#025A4E]">
        Roadmap
      </h1>
      <p class="mt-1 text-sm">
        Learning path recomendation and free course playlist
      </p>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <Icon name="uil:html5" />
      <h1 class="ml-1">HTML</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-left
    >
      <Icon name="uil:css3-simple" />
      <h1 class="ml-1">CSS DASAR</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <Icon name="uil:css3-simple" />
      <h1 class="ml-1">CSS Layouting</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-left
    >
      <Icon name="uil:css3-simple" />
      <h1 class="ml-1">CSS 3</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <h1 class="ml-1">Bootstrap</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-left
    >
      <Icon name="uil:css3-simple" />
      <h1 class="ml-1">Flexbox CSS</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <Icon name="uil:github" />
      <h1 class="ml-1">Git & Github</h1>
    </div>
    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-left
    >
      <h1 class="ml-1">Tailwind CSS</h1>
    </div>

    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <Icon name="uil:java-script" />
      <h1 class="ml-1">Javascipt Dasar</h1>
    </div>
    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-right
    >
      <Icon name="uil:java-script" />
      <h1 class="ml-1">Javascript DOM</h1>
    </div>
    <div
      class="font-semibold sm:w-[50%] w-[80%] bg-white rounded-xl px-5 h-[40px] flex items-center my-1 hover:drop-shadow-xl transition-transform hover:scale-105"
      v-motion-slide-visible-left
    >
      <Icon name="uil:java-script" />
      <h1 class="ml-1">Javascript Lanjutan</h1>
    </div>
  </div>
</template>
