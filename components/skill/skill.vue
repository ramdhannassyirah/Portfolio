<template>
  <div
    class="bg-[#025A4E] w-[150px] h-[40px] box-border rounded-full flex justify-center items-center"
  >
    <p class="font-semibold text-[13px] sm:text-xl text-[#ffffff]">
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
