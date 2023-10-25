<template>
  <div
    class="bg-[#ffffff] w-[150px] h-[40px] box-border rounded-full flex justify-center items-center"
  >
    <p class="font-semibold text-[13px] sm:text-xl text-[#025A4E]">
      {{ name }}
    </p>
  </div>
</template>

<script>
export default {
  props: {
    name: String, // Perbaikan: Menggunakan tipe data "String"
  },
};
</script>
