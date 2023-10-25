<template>
  <div
    class="bg-[#025A4E] w-[150px] h-[40px] rounded-full flex justify-center items-center"
  >
    <h1 class="font-semibold text-[#ffffff]">{{ name }}</h1>
  </div>
</template>

<script>
export default {
  props: {
    name: String, // Perbaikan: Menggunakan tipe data "String"
  },
};
</script>
