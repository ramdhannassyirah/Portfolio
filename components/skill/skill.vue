<template>
  <div
    class="bg-[#ffffff] w-[150px] h-[40px] box-border rounded-full flex justify-center items-center"
  >
    <h1 class="font-semibold text-[#025A4E]">{{ name }}</h1>
  </div>
</template>

<script>
export default {
  props: {
    name: String, // Perbaikan: Menggunakan tipe data "String"
  },
};
</script>
