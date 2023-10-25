<template>
  <div
    class="w-96 h-96 rounded-3xl sm:h-[400px] sm:w-[600px] sm:overflow-hidden card"
  >
    <div
      class="flex flex-col-reverse items-center py-10 text-center sm:flex-row sm:justify-between"
    >
      <div
        class="flex items-center justify-center my-2 text-center cursor-pointer rounded-xl"
      >
        <Icon name="uil:link" />
        <a class="mx-1 text-lg font-semibold hover:underline" :href="href"
          >Link</a
        >
      </div>
      <div class="">
        <h4 class="font-medium font-roboto">Project</h4>
        <h1 class="text-xl font-semibold font-playpen">{{ name }}</h1>
      </div>
    </div>
    <div class="zoom-on-hover">
      <a :href="href"> <img class="rounded-xl" :src="image" alt="" /></a>
    </div>
  </div>
</template>

<style>
.zoom-on-hover {
  transition: transform 0.3s; /* Animasi zoom selama 0.3 detik */
}

.zoom-on-hover:hover {
  transform: scale(1.1); /* Zoom gambar sebesar 110% saat mengarahkan kursor */
}
.card {
  transition: transform 0.3s, box-shadow 0.3s; /* Animasi transformasi dan bayangan selama 0.3 detik */
}

.card:hover {
  transform: scale(1.1); /* Scaling saat hover sebesar 110% */
  box-shadow: 0px 0px 50px 2px rgba(0, 0, 0, 0.4); /* Bayangan saat hover */
}
</style>
<script>
export default {
  props: {
    image: null,
    name: String,
    href: String,
  },
};
</script>
