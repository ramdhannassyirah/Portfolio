<template>
  <div
    class="container w-96 h-96 rounded-3xl sm:h-[400px] sm:w-46 overflow-hidden card"
  >
    <div class="p-10 text-center sm:text-right">
      <h4 class="font-medium font-roboto">Project</h4>
      <h1 class="text-xl font-semibold font-playpen">Article</h1>
    </div>
    <div class="zoom-on-hover">
      <img class="rounded-xl" src="http://source.unsplash.com/random" alt="" />
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
  box-shadow: 0px 0px 55px 2px rgba(0, 0, 0, 0.5); /* Bayangan saat hover */
}
</style>
