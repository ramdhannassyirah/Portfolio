<template>
  <nav class="pt-10">
    <div class="container flex justify-around mx-auto w-96 font-semi bold">
      <div class="">
        <a href="/" class=""
          >Work
          <span class="p-2 py-1 text-center text-white rounded bg-[#025A4E]"
            >/</span
          ></a
        >
      </div>
      <div class="">
        <a href="/about">About</a>
      </div>
      <div class="">
        <NuxtLink to="/roadmap">Roadmap</NuxtLink>
      </div>
      <div class="">
        <a href="">Notes</a>
      </div>
      <div class="">
        <NuxtLink to="/contact">Contact</NuxtLink>
      </div>
    </div>
  </nav>
</template>
